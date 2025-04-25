# HTTP 1.0

## 📌 Introduction
HTTP 1.0 was introduced in 1996 and marked a significant evolution from HTTP 0.9. For the first time, it introduced headers, status codes, and support for transmitting different types of media beyond just plain HTML. This version made the web more interactive and programmable.

---

## 🚀 Key Features
- Support for **HTTP headers** in both requests and responses.
- Introduction of **status codes** like `200 OK`, `404 Not Found`, etc.
- Multiple **MIME types** (images, scripts, etc.).
- Support for **POST and HEAD** methods.
- Basic caching with headers like `Expires`.
- HTTP version explicitly mentioned in the request (`HTTP 1.0`).

---

## ❗ Problems in HTTP 0.9
1. **Only one method (GET):** No support for POST, PUT, DELETE, etc.
2. **No HTTP headers:** No way to describe content type, language, caching rules, etc.
3. **No metadata or status codes:** No 404 Not Found or 200 OK – made error handling hard.
4. **Limited to plain HTML only:** Cannot transfer images, scripts, or styles.
5. **No persistent connections:** Connection closed after every request, making it inefficient.

---

## ✅ How New Versions Solved It
### HTTP 1.0 introduced:
- HTTP versioning in the request (`GET /index.html HTTP 1.0`)
- Response headers (like `Content-Type`, `Content-Length`)
- Status codes (`200 OK`, `404 Not Found`)
- Support for multiple content types

This made web communication richer and more flexible.

---

## 🧾 Conclusion
HTTP 1.0 was a turning point for the web, enabling more than just static HTML pages. It introduced the structure that future versions would build upon. However, its inefficiencies in connection management and caching led to the much-needed improvements in HTTP 1.1.
