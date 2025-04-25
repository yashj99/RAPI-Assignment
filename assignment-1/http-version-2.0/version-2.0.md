# HTTP 2

## 📌 Introduction
HTTP 2, released in 2015 (RFC 7540), was the first major update to the HTTP protocol since 1997. It was designed to overcome the inefficiencies and performance bottlenecks of HTTP 1.1, especially in delivering complex, resource-heavy modern websites.

HTTP 2 introduced binary framing, multiplexing, and header compression to improve latency and reduce overhead.

---

## 🚀 Key Features
- **Binary protocol**: More compact and easier for machines to parse.
- **Multiplexing**: Multiple requests/responses on a single TCP connection, eliminating head-of-line blocking at the application layer.
- **HPACK Header Compression**: Reduces redundancy in headers.
- **Stream Prioritization**: Resources can be loaded based on importance.
- **Server Push**: Server sends resources before client requests them.
- **TLS Encryption**: Not mandatory in spec, but all major browsers require HTTPS for HTTP 2.

---

## ❗ Problems in HTTP 1.1
1. **Head-of-line blocking:** Pipelining requests didn’t fully solve the blocking issue.
2. **Limited parallelism:** Still largely sequential and not optimized for many resources.
3. **Overhead:** Headers repeated with every request (even on the same connection).

---

## ✅ How New Versions Solved It
### HTTP 2 introduced:
- **Binary framing layer:** More efficient than text-based parsing.
- **Full multiplexing:** Multiple requests/responses on a single connection without blocking.
- **Header compression** (HPACK).
- **Stream prioritization** for resource loading.

This drastically improved performance, especially for complex modern web apps.

---

## ❗ Problems in HTTP 1.1 Solved by HTTP 2
| HTTP 1.1 Limitation            | HTTP 2 Solution                          |
|-------------------------------|------------------------------------------|
| Sequential Request Handling   | Multiplexed streams over one connection  |
| Large Headers Repeated Often  | HPACK Header Compression                 |
| No Prioritization             | Stream prioritization                    |
| No Push Mechanism             | Server Push                              |
| Head-of-line blocking         | Solved at app layer (still exists in TCP)|

---

## 🧾 Conclusion
HTTP 2 revolutionized web performance with features like multiplexing and header compression. It addressed many of HTTP 1.1’s inefficiencies but was still constrained by TCP’s transport-layer limitations. These bottlenecks were finally resolved in HTTP 3, which uses UDP and the QUIC protocol for faster, smarter communication.