1. Never use context api values in the Parent component.
%[https://codesandbox.io/embed/contextapi-drawback-0-w0dicr?fontsize=14&hidenavigation=1&theme=dark]

in this example we have used the state value in the parent component and we are passing these state values to the child component through Provider.
Child component are consuming these counter value using Consumers. So whenever the Provider value changes the components who are consuming these Context will also re-render to receive the updated value.But some child component are not actually using these counter, but then also they are re-rendering, the reason is that while updating state we are updating it in the parent component thus all children will re-render.

ThirdSimpleComp is re-rendering as its consuming the context.
FourthSimpleComp is re-rendering becasuse the states are in the parent and parent is re-rendering, we can overcome the issue for FourthSimpleComp by implementing React.memo

But we cannot overcome this with React.memo for ThirdsimpleComp

The solution for this is to have the counter provider state in a separate Provider component like this

%[https://codesandbox.io/embed/contextapi-drawback-1-1l68lh?fontsize=14&hidenavigation=1&theme=dark]

In this example we have lifter all the states to a separate file or component and the component is a Provider component.Now in App.js we can consume the values of the Context but wait.... If we use Consumer in App.js then whenever context value change, App.js will re-render and it will cause all child component to re-render even though those child component are NOT using the context value.

To get out of this, we again created 1 component (Consumer component) where we will consume our context values.

It dosent matter how many component you have wrapped in inside the provider, if the child of the provider is consuming the context then it will re-render and if it is not consuming the context then it wont re-render even though it is wrapped inside the Provider.

`TestChildRender` component is also re-rendering because its a child component of a component which are re-rendering.

If you want to restrict `TestChildRender` form re-rendering, then we can use React.useMemo or we can use the concept of {children} to render the TestChildRender

In this approach for ForthSimpleComp also we dont need to wrap it in React.memo


If let sat FourthSimpleComp is wrapped in the Provider and FourthSimpleComp is also using the useContext hook then FourthSimpleComp will also re-render on context update.

if FourthSimpleComp is written outside the Provider then if we use useContext there then it will not receive the context as its outside the provider, and it will then not re-render.

NOTE: Well, this is the only good news so far. Only components that call useContext re-render whenever the context’s state changes.

2. is it necessecery to re-render the counter2 component when we increment counter1 ?

NO right,
If Countersecond component doesnot using counter1 then its bad practice to re-render that when counter 1 changes.

How we can overcome this.

By creating multiple Providers and wrap component with those required provider

%[https://codesandbox.io/s/contextapi-drawback-2-xvn7x4?file=/src/App.js]