# Example of using regular expressions in JavaScript

## 1. Checking for the presence of a substring in a string
```js
const searchString = 'Hello, World!';
const substring = 'World';

if (searchString.includes(substring)) {
   console.log(`Substring '${substring}' found in '${searchString}'.`);
} else {
   console.log(`Substring '${substring}' not found in '${searchString}'.`);
}
```

## 2. Search and replace
```js
const textToReplace = 'JavaScript is awesome!';
const replacedText = textToReplace.replace(/awesome/, 'amazing');
console.log(`Original text: ${textToReplace}`);
console.log(`Replaced text: ${replacedText}`);
```

## 3. Checking the email format
```js
const emailToValidate = 'example@email.com';
const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;

if (emailRegex.test(emailToValidate)) {
   console.log(`Email '${emailToValidate}' is valid.`);
} else {
   console.log(`Email '${emailToValidate}' is not valid.`);
}
```

## 4. Extracting a number from a string
```js
const stringWithNumber = 'The price is $25.99';
const extractedNumber = parseFloat(stringWithNumber.match(/\d+\.\d+/)[0]);
console.log(`Extracted number: ${extractedNumber}`);
```
