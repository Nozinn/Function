# JavaScript Data Types
JavaScript имеет динамическую типизацию и поддерживает примитивные и сложные (объектные) типы данных.
## Примитивные типы данных
Примитивные типы данных являются неизменяемыми (immutable) и передаются по значению.
1. **Number** – числовой тип данных (целые и десятичные числа)
   ```js
   let num = 42;
   let floatNum = 3.14;
   ```
2. **String** – строка текста, заключённая в кавычки
   ```js
   let str = "Hello, World!";
   ```
3. **Boolean** – логический тип (true/false)
   ```js
   let isActive = true;
   ```
4. **Undefined** – значение переменной, которой не присвоено значение
   ```js
   let notDefined;
   console.log(notDefined); // undefined
   ```
5. **Null** – отсутствие значения
   ```js
   let empty = null;
   ```
6. **Symbol** – уникальный и неизменяемый идентификатор
   ```js
   let sym = Symbol("id");
   ```
7. **BigInt** – числа, превышающие предел типа Number
   ```js
   let bigNumber = 9007199254740991n;
   ```
## Сложные (объектные) типы данных
Объекты передаются по ссылке и могут изменяться.
1. **Object** – коллекция пар "ключ-значение"
   ```js
   let user = { name: "Alice", age: 25 };
   ```
2. **Array** – упорядоченный список значений
   ```js
   let numbers = [1, 2, 3, 4, 5];
   ```
3. **Function** – подтип объекта, вызываемый с аргументами
   ```js
   function greet(name) {
       return "Hello, " + name;
   }
   ```
4. **Date** – объект для работы с датами
   ```js
   let now = new Date();
   ```

5. **RegExp** – регулярные выражения
   ```js
   let regex = /hello/i;
   ```

## Проверка типа данных
Для определения типа данных используется оператор `typeof`:
```js
console.log(typeof 42); // "number"
console.log(typeof "Hello"); // "string"
console.log(typeof true); // "boolean"
console.log(typeof undefined); // "undefined"
console.log(typeof null); // "object" (известная ошибка в JS)
console.log(typeof Symbol("id")); // "symbol"
console.log(typeof 10n); // "bigint"
console.log(typeof {}); // "object"
console.log(typeof []); // "object"
console.log(typeof function(){}); // "function"
```
## Заключение
JavaScript имеет 7 примитивных и несколько сложных типов данных. Важно понимать их отличия и особенности работы, особенно с точки зрения передачи по значению и по ссылке.

