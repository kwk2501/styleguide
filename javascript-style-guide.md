# RecordFarm Javascript 스타일 가이드

## 목차
  1. [서식 (formatting)](#formatting)
    2. [공백 (Whitespace)](#whitespace)
  1. [References](#references)
  1. [Objects](#objects)
  1. [Arrays](#arrays)
  1. [Contributors](#contributors)
  1. [License](#license)


## 1. 서식 (formatting)

### 1.1. 공백 (Whitespace)

  <a name="Whitespace--2칸 들여쓰기"></a><a name="1.1"></a>
  - [1.1.1.](#Whitespace--2칸 들여쓰기) **2칸 들여쓰기 (2 spaces for indentation)**: 2칸 들여쓰기를 하며, 탭에는 스페이스 2개를 설정해 주십시오.
  

    ```javascript
    // bad
    (function () {
    ∙∙∙∙const name = 'RecordFarm';
    })()

    // bad
    (function () {
    ∙∙∙∙const name = 'RecordFarm';
    }());
    
    // good
    (function () {
    ∙∙const name = 'RecordFarm';
    }());
    ```


  <a name="Whitespace--brace"></a><a name="1.2"></a>
  - [1.1.2.](#Whitespace--brace) **중괄호 (brace)**: 중괄호 앞에는 1칸 띄어쓰기 해주십시오
        ```javascript
    // bad
    function test(){
      const name = 'RecordFarm';
    }

    // good
    function test() {
      const name = 'RecordFarm';
    }
    ```



### 2. 세미콜론 (Semicolons)
    <a name="formatting--semicolon"></a><a name="1.1"></a>
  - [1.2.1.](#formatting--semicolon) **세미콜론을 사용하세요 (Use semicolon)**: 모든 문장에는 세미콜론을 붙여주세요.
      ```javascript
    // bad
    (function () {
      const name = 'RecordFarm'
      return name
    })()

    // good
    (function () {
      const name = 'RecordFarm';
      return name;
    }());
    ```
    
  
  
  
  
  
  
  
  
  
  
    

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
