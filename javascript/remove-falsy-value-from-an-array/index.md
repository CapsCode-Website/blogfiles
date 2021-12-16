var a = [1, 2, "b", 0, {}, "", NaN, 3, undefined, null, 5];
a.filter(Boolean)
a.filter(Number)

function Fun(a){
return a>2
}
a.filter(Fun)

Boolean(NaN)
