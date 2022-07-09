---
id: y1ng2qxm7ukl5sce22whs3d
title: Performance
desc: ''
updated: 1657372166115
created: 1657371770600
---

# Rate Limiting

## Debouncing

- limiting the rate of execution of a particular function
- used in search bars etc.
- I have normally used lodash Debouncing

### Create debounce fun from scratch

```js
const handleChange = (e) => {
    console.log(e.target.value);
}
const debounce = (fn, wait) => {
    let timer;
    return function(...args) {
        const context = this; // maintains the context, so that the fn is called within the same lexical environment with same arguments as it was running before wrapping it around a debounce function.
        clearTimeout(timer) // clear timer in subsequent keystrokes.
         timer = setTimeout(() => {
            fn.apply(context, args)
        }, wait);
    }
}
const optiminzedFn = debounce(handleChange)
```

## Throttling