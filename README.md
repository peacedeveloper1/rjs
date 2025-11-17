
# ⭐ **README.md **

(*RJS — Revolution JavaScript Edition*)

---

# RJS — Revolution JavaScript

*A lightweight JavaScript-oriented language with a clean, expressive syntax.*

RJS (Revolution JavaScript) is a tiny mini-language that compiles directly to modern JavaScript.
It removes noise, reduces boilerplate, and brings a fast, reactive flow to everyday scripting.

RJS has **no runtime**, **no dependencies**, and runs anywhere JavaScript runs.


---

# 🌐 Live Demo

Try RJS instantly in your browser:

👉 **[https://peacedeveloper1.github.io/rjs/rjs-demo-table.html](https://peacedeveloper1.github.io/rjs/rjs-demo-table.html)**

No install required — just click and run.

---

## ✨ Features

### **Minimal variable declarations**

```rjs
x:Int := 10       // let
pi:Float :: 3.14  // const
msg:String := "hello"
```

### **Compact function syntax**

```rjs
fn add(a:Int, b:Int) = a + b
```

Block form:

```rjs
fn main()
  log "Hello"
end
```

### **RJD Table Literal (array-of-objects)**

```rjs
users:User[] :: [<
  id  name      age
  1   "Alice"   30
  2   "Bob"     25
>]
```

### **Inline actions (`if ->`)**

```rjs
if value > 0 -> log "Positive"
```

### **Zero-noise block structure**

```rjs
if x > 10
  log "big"
else
  log "small"
end
```

### **Browser loader**

```html
<script src="rjs-compiler.min.js"></script>
<script> RJS.load("main.rjs"); </script>
```

---

# 🚀 Getting Started

## 📦 Install (Local Development)

RJS demos require a basic web server (due to browser `fetch()` restrictions).

Install dependencies:

```bash
npm install
```

Run a local development server:

```bash
npm run dev
```

The project will be available at:

```
http://localhost:8080/
```

---

# 📁 Project Structure

```
.
├── demo_ui_app.rjs
├── rjs-compiler.min.js
├── rjs-demo-table.html
├── package.json
└── node_modules/
```

* **rjs-compiler.min.js** — the RJS → JavaScript compiler
* **demo_ui_app.rjs** — sample RJS script
* **rjs-demo-table.html** — browser demo using RJS.load

---

# 🧪 Example: Loading an RJS file in the Browser

```html
<script src="rjs-compiler.min.js"></script>

<script>
  RJS.load("demo_ui_app.rjs");
</script>
```

---

# 📜 Philosophy

RJS is designed to feel like **pseudocode that runs**.

* Clean syntax
* Predictable JavaScript output
* No runtime cost
* Ideal for small tools, prototypes, demos, and DSL-style workflows

The goal:

> “Let your ideas move faster than the boilerplate.”

---

# 🛠 Roadmap

* VSCode syntax highlighting
* Improved compile errors
* Plugin-based compile passes
* Optional macro sugar
* Type-aware tooling

