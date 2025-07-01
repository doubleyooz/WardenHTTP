Here’s a **fancy and professional `README.md`** for your NPM package, themed like an old gatekeeper’s scroll guarding the realms of HTTP status clarity:

---

````markdown
# 🏰 Warden HTTP

**Warden HTTP** is a collection of standardized **HTTP response constants and descriptions**, designed to bring clarity, consistency, and a touch of medieval elegance to your API responses. No magic, no runtime – just pure, readable, constant values.

> ⚔️ "He who guards the gate must know its every cry."

---

## ✨ Features

- 📜 Descriptive constants for all major HTTP status codes
- 🔒 Fully immutable — exported as `const`
- 🧙 Clean, documented, and zero-dependency
- 🏗️ Great for standardizing internal tools, APIs, and logging

---

## 📦 Installation

```bash
npm install warden-http
# or
yarn add warden-http
````

---

## 🔍 Usage

```ts
import { OK, NOT_FOUND } from 'warden-http';

function handler(req, res) {
  res.status(200).send(OK); // "OK: The request has succeeded."
}
```

Or simply:

```ts
res.status(404).send(NOT_FOUND); 
// "Not Found: The requested resource could not be found on this server."
```

---

## 📚 Exports

All constants follow the `UPPER_SNAKE_CASE` convention and are directly exported. You get **two flavors**:

### 1. 🧾 Description Strings

```ts
import { BAD_REQUEST } from 'warden-http';

console.log(BAD_REQUEST);
// "Bad Request: The server could not understand the request due to invalid syntax."
```

### 2. 🔢 Numeric Status Codes

```ts
import { BAD_REQUEST as BAD_REQUEST_CODE } from 'warden-http/codes';

console.log(BAD_REQUEST_CODE);
// 400
```

---

## 🗃️ Available Statuses

This package includes **all major** informational, success, redirection, client, and server error codes:

| Code | Constant                | Description                            |
| ---- | ----------------------- | -------------------------------------- |
| 200  | `OK`                    | "OK: The request has succeeded."       |
| 201  | `CREATED`               | "Created: A new resource was made."    |
| 204  | `NO_CONTENT`            | "The server is not returning content." |
| 400  | `BAD_REQUEST`           | "Invalid syntax in request."           |
| 401  | `UNAUTHORIZED`          | "Auth is required or failed."          |
| 404  | `NOT_FOUND`             | "Resource could not be found."         |
| 500  | `INTERNAL_SERVER_ERROR` | "The server encountered an error."     |

*... and many more. Full list in `src/index.ts`.*

---

## 🧱 Why Use This?

* No need to memorize status messages
* Improve log readability
* Eliminate hardcoded strings
* Keep your code semantically expressive

---

## 🏁 Roadmap

* [ ] Export grouped enums: `Http2xx`, `Http4xx`, etc.
* [ ] Internationalized versions (e.g., `pt-BR`, `fr`)
* [ ] Express middleware using these messages

---

## 🏷️ License

MIT — yours to forge and reuse in your kingdom of code.

---

## 🔖 Tip from the Gatekeeper

> “A wise dev never hardcodes a message twice.”

🧙‍♂️ Use `warden-http` and stand guard over your response semantics.

---

```

Let me know your final package name and I’ll swap in all mentions (currently "warden-http") to match!
```
