# BFE.dev

Visualizations to solutions, made with [excalidraw-claymate](https://github.com/dai-shi/excalidraw-claymate).

And some explaining videos, blogs, etc.

## JavaScript Coding Questions

### [`curry()` with placeholder](https://bigfrontend.dev/problem/implement-curry-with-placeholder)

![excalidraw-claymate](https://github.com/yuleicul/bfe.dev/assets/27288153/2e0e14a4-fd79-48da-bea5-0c73a01e9aea)

### [Basic `throttle()`](https://bigfrontend.dev/problem/implement-basic-throttle)

throttled Kirby:
    
![excalidraw-claymate-throttle](https://github.com/yuleicul/bfe.dev/assets/27288153/72bdc0f5-3bf5-49f1-883d-7a79956b5b4e)

more to read/watch:
- code: https://youtu.be/cjIswDCKgu0
- visualized: https://css-tricks.com/debouncing-throttling-explained-examples/

### [Can you `shuffle()` an array?](https://bigfrontend.dev/problem/can-you-shuffle-an-array)

```javascript
// Fisher-Yates
function shuffle(arr) {
  for(let i = arr.length - 1; i >= 0; i--) {
    const index = Math.floor(Math.random() * (i + 1))
    ;[arr[i], arr[index]] = [arr[index], arr[i]]
  }
  return arr
}

// Why this doesn't work?
// There's no problem with `const index = Math.floor(Math.random() * arr.length)`
// Every position does get a correct possibility,
// but the number in the position changes because of `splice`
// Fisher-Yates can make sure the number in some position keep the same
// function shuffle(arr) {
//   const result = []
  
//   const length = arr.length
//   for (let i = 0; i < length; i++) {
//     const index = Math.floor(Math.random() * arr.length)
//     result.push(arr[index])
//     arr.splice(index, 1)
//   }

//   return result
// }
```

### [Decode message](https://bigfrontend.dev/problem/decode-message)

![excalidraw-claymate-decoder](https://github.com/yuleicul/bfe.dev/assets/27288153/3cd877a2-6a54-407c-8a74-a9f62ba9ac2b)

### [Detect data type in JavaScript](https://bigfrontend.dev/problem/detect-data-type-in-JavaScript)
![image](https://github.com/yuleicul/bfe.dev/assets/27288153/773accde-0681-4fc9-b9c9-1307e293d231)
