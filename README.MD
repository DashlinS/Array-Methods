#
Array - Methods
/* map 
reduce 
filter 
forEach 
sort 
slice 
pop 
shift 
push 
unshift 
includes 
indexOf 
every */

let array = [1,2,3,4,5]
let arrayTwo = ['h','e','l','l','o']

## Map Method
// map method does a function once for each element in an array and creates a new array without modifying the original. The map method has a time complexity of O(n)
console.log('Map Method')
console.log(array.map(element => element * 2))
console.log(arrayTwo.map(element => element.toUpperCase()))

## Reduce Method
// reduce method does a function for each element in an array, reducing it to a single value. Reduce has a time complexity of O(n)
console.log('Reduce Method')
console.log(array.reduce((acc, val) => acc * val, 1))
console.log(arrayTwo.reduce((acc, val) => acc + val))

## Filter Method
// filter method filters the array using a function provided given that it is true. Filter method has a time complexity of O(n)
console.log('Filter Method')
console.log(array.filter(element => element % 2 === 0))
console.log(arrayTwo.filter(element => arrayTwo.indexOf(element) !== arrayTwo.lastIndexOf(element)))

## forEach Method
// forEach method does a function once for each element in an array, modifies the original array. The forEach method has a time complexity of O(n)
console.log('ForEach Method')
array.forEach(element => {
  console.log(element - 1)
})
arrayTwo.forEach(element => {
  console.log(element.toUpperCase())
})

## Sort Method
// sort method sorts the array, modifying it. If not specified, it will modify by the unicode values. Sort method has a time complexity of O(n * log n)
console.log('Sort Method')
// console.log(array.sort((a,b) => b - a))
// console.log(arrayTwo.sort((a,b) => b - a))

## Slice Method
// slice method slices the array/string from one point to another and returns the sliced part. Slice method has a time complexity of O(n)
console.log('Slice Method')
console.log(array.slice(2,4))
console.log(arrayTwo.slice(1,2))

## Pop Method
// pop method removes the last element in an array and returns that element. pop method has a time complexity of O(1)
console.log('Pop Method')
console.log(array.pop())
console.log(arrayTwo.pop())

## Shift Method
// shift method removes the first element in an array and returns that element. Shift method has a time complexity of O(n)
console.log('Shift Method')
console.log(array.shift())
console.log(arrayTwo.shift())

## Push Method
// push method adds an element to the end of an array and returns the new length. push method has a time complexity of O(1)
console.log('Push Method')
console.log(array.push(5))
console.log(arrayTwo.push('!','!'))

## unshift Method
// unshift method adds an element to the beginning of an array and returns the array. Unshift method has a time complexity of O(n)
console.log('unshift Method')
console.log(array.unshift(0))
console.log(arrayTwo.unshift('!'))

## includes Method
// includes method is a boolean that checks if an element exists in an array. includes method has a time complexity of O(n)
console.log('includes Method')
console.log(array.includes(4))
console.log(arrayTwo.includes('l'))

## indexOf Method
// indexOf method looks for the index of the target element, returns -1 if not found. indexOf method has a time complexity of O(n)
console.log('indexOf Method')
console.log(array.indexOf(3))
console.log(arrayTwo.indexOf('e'))

## every Method
// every method boolean that checks if every element passes a test. every method has a time complexity of O(n)
console.log('every Method')
console.log(array.every(element => typeof(element) === 'number'))
console.log(arrayTwo.every(element => typeof(element) === 'boolean'))