# Sorting

> A *sorting algorithm* is basically an algorithm that, given a list of records
containing a key and some data, reorders the list so that the keys are in non
decreasing order (no key is smaller than its preceding key), and the output list
is a permutation of the input list, retaining all original records.

## The Sorting Problem

### Internal vs External Sorting

- **Internal**: can all be stored in memory
- **External**: must reside in a storage device

### Adaptive Sorting

> If the algorithm takes advantage of whatever existing order already exists in
its input

## Sorting with Comparisons

### Bubbling Up and Down

#### Bubble Sort

```js
const bubbleSort = (arr, from = 0, to = arr.length -1) => {
    for (let j = to; j > from; j--){
        for (let i = from; i < j; i++){
            if (arr[i] > arr[i +1]) {
                [arr[i], arr[i+1]] = [arr[i +1], arr[i]];
            }
        }
    }
    return arr
}
```

#### Sinking Sort and Shuttle Sort

```js
```
