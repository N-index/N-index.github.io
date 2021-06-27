# It's my github page

[comment]: <> (![图片]&#40;http://germ.run/static/images/wearMask.png =250x250&#41;)
<img src="http://germ.run/static/images/wearMask.png" height="200" alt="Figure 1-1">


```javascript
// quick sort
function quick_sort(arr){
    if (arr.length <= 1){
        return arr;
    }
    const pivot = arr[0];
    const left = [],right = [];
    arr.forEach(e=>{
        if (e < pivot) left.push(e);
        if (e > pivot) right.push(e);
    });
    return [...quick_sort(left), pivot, ...quick_sort(right)];
}
```