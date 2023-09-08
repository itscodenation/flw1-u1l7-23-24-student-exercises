# Lesson 1.7 : DOM Manipulation, Part 2 & Project Work Time

## ⌨️ String Interpolation:

- Embedding values within a string is done using **string interpolation**.
- This is achieved using **template literals**.
  
  ```javascript
  let name = 'John';
  let greeting = `Hello, ${name}!`;
  console.log(greeting); // Outputs: Hello, John!
  ```

  - Template literals are enclosed by backticks (` `` `).
  - Variables or expressions are placed inside `${...}`.
  
  ```javascript
  let a = 10;
  let b = 20;
  let result = `Sum of a and b is ${a + b}.`;
  console.log(result); // Outputs: The sum of a and b is 30.
  ```

## 📦 Storing Input Values:

- **Input fields** allow websites to gather data from users.
  
  ```html
  <input class="user-input" placeholder="Email">
  <button>Log in</button>
  ```

- With JavaScript, you can extract the value of the input using the `.value` method.
  
  ```javascript
  let button = document.querySelector("button");
  button.addEventListener("click", function() {
    let userInput = document.querySelector("input").value;
    console.log(userInput);
  });
  ```

## ✨ DOM & Styling:

- Manipulate page styling using JavaScript and the `.style` property.
  
  ```javascript
  let header = document.querySelector("h1");
  header.style.backgroundColor = "black";
  header.style.color = "lightGreen";
  ```

- Be aware of **camelCase** for hyphenated properties in JS:
  - `background-color` becomes `backgroundColor`.
  - `font-size` becomes `fontSize`.
