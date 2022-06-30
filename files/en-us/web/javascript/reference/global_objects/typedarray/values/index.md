---
title: TypedArray.prototype.values()
slug: Web/JavaScript/Reference/Global_Objects/TypedArray/values
tags:
  - ECMAScript 2015
  - Iterator
  - JavaScript
  - Method
  - Prototype
  - TypedArray
  - TypedArrays
---
{{JSRef}}

The **`values()`** method returns a new `Array Iterator` object that contains the values for each index in the array.

{{EmbedInteractiveExample("pages/js/typedarray-values.html")}}

## Syntax

    arr.values()

### Return value

A new **`Array Iterator`** object.

## Examples

### Iteration using `for...of` loop

```js
var arr = new Uint8Array([10, 20, 30, 40, 50]);
var eArray = arr.values();
// your browser must support for..of loop
// and let-scoped variables in for loops
for (let n of eArray) {
  console.log(n);
}
```

### Alternative iteration

```js
var arr = new Uint8Array([10, 20, 30, 40, 50]);
var eArr = arr.values();
console.log(eArr.next().value); // 10
console.log(eArr.next().value); // 20
console.log(eArr.next().value); // 30
console.log(eArr.next().value); // 40
console.log(eArr.next().value); // 50
```

## Specifications

| Specification                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------- |
| {{SpecName('ESDraft', '#sec-%typedarray%.prototype.values', '%TypedArray%.prototype.values()')}} |

## Browser compatibility

{{Compat("javascript.builtins.TypedArray.values")}}

## See also

- [JavaScript typed arrays](/en-US/docs/Web/JavaScript/Typed_arrays)
- {{jsxref("TypedArray")}}
- {{jsxref("TypedArray.prototype.entries()")}}
- {{jsxref("TypedArray.prototype.keys()")}}
- {{jsxref("TypedArray.prototype.@@iterator()", "TypedArray.prototype[@@iterator]()")}}
