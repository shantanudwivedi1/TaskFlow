# JavaScript Objects and JSON

## 1. What is a JavaScript object?

An object stores related information using key-value pairs.

```javascript
const task = {
  id: 1,
  title: "Learn React",
  completed: false
};

console.log(task.title);
```

Output:
```text
Learn React
```

## 2. What is JSON?

JSON stands for JavaScript Object Notation. It is a text format used to exchange data between applications.

## 3. Convert JavaScript data into JSON

Use `JSON.stringify()`.

```javascript
const task = {
  id: 1,
  title: "Learn React",
  completed: false
};

const jsonData = JSON.stringify(task);
console.log(jsonData);
```

## 4. Convert JSON text into JavaScript data

Use `JSON.parse()`.

```javascript
const jsonData = '{"id":1,"title":"Learn React","completed":false}';

const task = JSON.parse(jsonData);
console.log(task.title);
```

Output:
```text
Learn React
```

## 5. Arrays containing objects

An array can store multiple objects.

```javascript
const tasks = [
  { id: 1, title: "Learn React" },
  { id: 2, title: "Learn Node.js" }
];

console.log(tasks[0].title);
console.log(tasks[1].title);
```

Output:
```text
Learn React
Learn Node.js
```

Remember:
- `JSON.stringify()` converts JavaScript data into JSON text.
- `JSON.parse()` converts valid JSON text into JavaScript data.
- Array indexes start at `0`.
- Use `tasks[0].title` to access the first task's title.