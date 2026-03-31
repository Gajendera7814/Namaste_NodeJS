
---

# Introduction to Node.js

## What is Node.js

**Node.js** is an **open-source, cross-platform JavaScript runtime environment** that allows developers to execute JavaScript code **outside the web browser**.

It is built on the **Google Chrome V8 engine** and is mainly used for building **fast, scalable, and data-intensive server-side applications**.

Node.js enables developers to use JavaScript for both frontend and backend development.

---

# JavaScript Runtime Environment

A **runtime environment** is the environment where a program executes.

JavaScript usually runs in **web browsers** like:

* Chrome
* Firefox
* Edge

But **Node.js allows JavaScript to run outside the browser**, such as on a **server or local machine**.

---

# V8 Engine

Node.js is built on the Google Chrome V8 engine.

The **V8 Engine** is a JavaScript engine developed by Google.

The V8 engine:

* Compiles JavaScript into **machine code**
* Executes the code very **fast**
* Uses **Just-In-Time (JIT) compilation** for better performance

Node.js uses the **Chrome V8 Engine** to run JavaScript.

---

# Open Source

**Open source** means the **source code is publicly available**.

This means:

* The source code is publicly available
* Developers can view the code
* Developers can modify the code
* Developers can contribute to the project

---

# Cross Platform

Node.js is cross-platform, which means it can run on different operating systems without requiring major changes.

Supported platforms include:

* Windows
* macOS
* Linux

---

# Why Node.js is Used

Node.js is used to build:

* Web servers
* APIs
* Real-time applications
* Streaming apps
* Chat applications

Examples:

* Netflix
* PayPal
* Uber
* Trello

---

## Key Features of Node.js

### 1. Asynchronous and Non-Blocking

Node.js uses non-blocking I/O operations, allowing it to handle multiple requests simultaneously.

### 2. Event Driven

Node.js follows an event-driven architecture which improves application performance.

### 3. Fast Execution

Because it uses the V8 JavaScript engine, Node.js executes code very efficiently.

### 4. Scalable

Node.js is capable of handling a large number of concurrent connections.

### 5. Single Threaded Event Loop

Node.js uses a single-threaded event loop architecture to handle multiple operations efficiently.

---

# Built-in Modules (APIs)

Node.js provides **built-in modules** that help developers perform common tasks.

Examples:

| Module | Use                    |
| ------ | ---------------------- |
| fs     | File system operations |
| http   | Create web servers     |
| path   | Work with file paths   |
| os     | System information     |
| events | Event handling         |

Example:

```js
const fs = require('fs');

fs.readFile('file.txt', 'utf8', (err, data) => {
    console.log(data);
});
```

---

## Built-in Modules

Node.js provides several built-in modules to perform common tasks.

Examples:

| Module | Description                           |
| ------ | ------------------------------------- |
| http   | Used to create web servers            |
| fs     | Used to work with file systems        |
| path   | Used to handle file paths             |
| os     | Provides operating system information |
| events | Used for event handling               |

Example:

```javascript
const fs = require("fs");

fs.readFile("file.txt", "utf8", (err, data) => {
    if (err) {
        console.log(err);
    } else {
        console.log(data);
    }
});
```

---

## Simple Node.js Server Example

```javascript
const http = require("http");

const server = http.createServer((req, res) => {
    res.write("Hello from Node.js");
    res.end();
});

server.listen(3000, () => {
    console.log("Server running on port 3000");
});
```

Open your browser and visit:

http://localhost:3000

---

# Node.js is Not a Programming Language

Node.js is **not a programming language**.

It is a **runtime environment** that allows JavaScript to run **outside the browser**.

---
