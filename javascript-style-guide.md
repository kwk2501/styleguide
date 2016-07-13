# RecordFarm Javascript 스타일 가이드

## 목차
  1. [서식 (formatting)](#formatting)
    2. [hh](#sagf)
  1. [References](#references)
  1. [Objects](#objects)
  1. [Arrays](#arrays)
  1. [Contributors](#contributors)
  1. [License](#license)


## 서식 (formatting)

  <a name="formatting--2칸 들여쓰기"></a><a name="1.1"></a>
  - [1.1](#formatting--2칸 들여쓰기) **formatting--2칸 들여쓰기**: When you access a primitive type you work directly on its value.

    + `string`
    + `number`
    + `boolean`
    + `null`
    + `undefined`

    ```javascript
    const foo = 1;
    let bar = foo;

    bar = 9;

    console.log(foo, bar); // => 1, 9
    ```

  <a name="types--complex"></a><a name="1.2"></a>
  - [1.2](#types--complex)  **Complex**: When you access a complex type you work on a reference to its value.

    + `object`
    + `array`
    + `function`

    ```javascript
    const foo = [1, 2];
    const bar = foo;

    bar[0] = 9;

    console.log(foo[0], bar[0]); // => 9, 9
    ```

**[⬆ back to top](#table-of-contents)**



## References
