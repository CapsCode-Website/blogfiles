# Turn your Create React App into a Progressive Web App in 100 seconds

[Progressive Web Apps](https://web.dev/progressive-web-apps/) (PWAs) let regular apps become accessible offline. They also have access to more features than regular apps.

React Apps need two features to become Progressive Web Apps.  
First, they need a service worker, which does work in the background of the app. Second, they need a `manifest.json` file in the public folder, which includes the name of the app, the home page, and icons.

If you're starting fresh, you can use the Create React App template `cra-template-pwa` (or `cra-template-pwa-typescript`) to bootstrap this process. If you want to create a React app from the start like this, use the command `npx create-react-app app-name --template cra-template-pwa` or `npx create-react-app app-name --template cra-template-pwa-typescript`.

But, if you're like me, you didn't think to add this template in the beginning, and are wondering how to add it to an existing app.

## [](https://dev.to/myfatemi04/turn-your-create-react-app-into-a-progressive-web-app-in-100-seconds-3c11#1-raw-manifestjson-endraw-)1. `manifest.json`

`manifest.json` goes in the `public` folder.

Most parts are self-explanatory. You can generate this file with websites like [Simicart's](https://www.simicart.com/manifest-generator.html/).

Here's an example. Note that this requires `favicon.ico`, `logo192.png`, and `logo512.png` to be available in the `public` folder.

```

{
    "short_name": "App",
    "name": "My App",
    "icons": [
        {
            "src": "favicon.ico",
            "sizes": "64x64 32x32 24x24 16x16",
            "type": "image/x-icon"
        },
        {
            "src": "logo192.png",
            "type": "image/png",
            "sizes": "192x192"
        },
        {
            "src": "logo512.png",
            "type": "image/png",
            "sizes": "512x512"
        }
    ],
    "start_url": ".",
    "display": "standalone",
    "theme_color": "#000000",
    "background_color": "#ffffff"
}



```

## [](https://dev.to/myfatemi04/turn-your-create-react-app-into-a-progressive-web-app-in-100-seconds-3c11#2-raw-serviceworkerjs-endraw-)2. `service-worker.js`

For a baseline, go to the [cra-template-pwa github](https://github.com/cra-template/pwa/tree/master/packages/cra-template-pwa-typescript/template/src).

Copy `service-worker.ts` and `serviceWorkerRegistration.ts` into the `src` folder.

Then, at the top of your `index.tsx` (or any entrypoint), import the service worker registration like so:

```

import * as serviceWorkerRegistration from './serviceWorkerRegistration';


```

At the bottom of your `index.tsx`, add the following code to opt into an "offline-first" app:

```

serviceWorkerRegistration.register();


```

[Learn more about PWAs](https://create-react-app.dev/docs/making-a-progressive-web-app/)
