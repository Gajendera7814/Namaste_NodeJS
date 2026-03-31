# Introduction to Node.js

## What is Node.js

**Node.js** is an <span style="color:#2ecc71"><b>open-source, cross-platform JavaScript runtime environment</b></span> that allows developers to execute JavaScript code <span style="color:#3498db"><b>outside the web browser</b></span>.

It is built on the <span style="color:#e67e22"><b>Google Chrome V8 engine</b></span> and is mainly used for building <span style="color:#9b59b6"><b>fast, scalable, and data-intensive server-side applications</b></span>.

Node.js enables developers to use JavaScript for <span style="color:#1abc9c"><b>both frontend and backend development</b></span>.

---

# JavaScript Runtime Environment

A <span style="color:#e74c3c"><b>runtime environment</b></span> is the environment where a program executes.

JavaScript usually runs in <span style="color:#3498db"><b>web browsers</b></span> like:

- Chrome  
- Firefox  
- Edge  

But <span style="color:#2ecc71"><b>Node.js allows JavaScript to run outside the browser</b></span>, such as on a <span style="color:#9b59b6"><b>server or local machine</b></span>.

---

# V8 Engine

Node.js is built on the <span style="color:#e67e22"><b>Google Chrome V8 engine</b></span>.

The <span style="color:#e67e22"><b>V8 Engine</b></span> is a JavaScript engine developed by Google.

The V8 engine:

- Compiles JavaScript into <span style="color:#2ecc71"><b>machine code</b></span>  
- Executes the code very <span style="color:#3498db"><b>fast</b></span>  
- Uses <span style="color:#9b59b6"><b>Just-In-Time (JIT) compilation</b></span> for better performance  

Node.js uses the <span style="color:#e67e22"><b>Chrome V8 Engine</b></span> to run JavaScript.

---

# Open Source

<span style="color:#2ecc71"><b>Open source</b></span> means the <span style="color:#3498db"><b>source code is publicly available</b></span>.

This means:

- Developers can <span style="color:#9b59b6"><b>view</b></span> the code  
- Developers can <span style="color:#e67e22"><b>modify</b></span> the code  
- Developers can <span style="color:#1abc9c"><b>contribute</b></span> to the project  

---

# Cross Platform

Node.js is <span style="color:#2ecc71"><b>cross-platform</b></span>, which means it can run on different operating systems without requiring major changes.

Supported platforms include:

- Windows  
- macOS  
- Linux  

---

# Why Node.js is Used

Node.js is used to build:

- Web servers  
- APIs  
- Real-time applications  
- Streaming apps  
- Chat applications  

Examples:

- Netflix  
- PayPal  
- Uber  
- Trello  

---

# Key Features of Node.js

### 1. Asynchronous and Non-Blocking

Node.js uses <span style="color:#e74c3c"><b>non-blocking I/O operations</b></span>, allowing it to handle <span style="color:#2ecc71"><b>multiple requests simultaneously</b></span>.

### 2. Event Driven

Node.js follows an <span style="color:#9b59b6"><b>event-driven architecture</b></span> which improves application performance.

### 3. Fast Execution

Because it uses the <span style="color:#e67e22"><b>V8 JavaScript engine</b></span>, Node.js executes code very efficiently.

### 4. Scalable

Node.js is capable of handling a <span style="color:#3498db"><b>large number of concurrent connections</b></span>.

### 5. Single Threaded Event Loop

Node.js uses a <span style="color:#e74c3c"><b>single-threaded event loop architecture</b></span> to handle multiple operations efficiently.

---

# Built-in Modules (APIs)

Node.js provides <span style="color:#2ecc71"><b>built-in modules</b></span> that help developers perform common tasks.

| Module | Use |
|------|------|
| fs | File system operations |
| http | Create web servers |
| path | Work with file paths |
| os | System information |
| events | Event handling |

Example:

```js
const fs = require("fs");

fs.readFile("file.txt", "utf8", (err, data) => {
    console.log(data);
});
```

---

# Simple Node.js Server Example

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

After running the file, open your browser and visit:

**http://localhost:3000**

---

# Node.js is Not a Programming Language

<span style="color:#e74c3c"><b>Node.js is NOT a programming language.</b></span>

It is a <span style="color:#2ecc71"><b>JavaScript runtime environment</b></span> that allows JavaScript to run <span style="color:#3498db"><b>outside the web browser</b></span>.

This means developers can use JavaScript to build:

- Web servers  
- APIs  
- Real-time applications  
- Backend services  

---
