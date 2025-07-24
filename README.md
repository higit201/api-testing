# 🔍 API Testing Collection using Postman & Newman

This repository contains a set of automated test cases for RESTful API endpoints using [Postman](https://www.postman.com/) and executed via [Newman](https://www.npmjs.com/package/newman) — Postman's command-line companion.

---

## 📁 Project Overview

This project tests the sample REST API provided by **JSONPlaceholder**:  
**`https://jsonplaceholder.typicode.com/posts`**

It includes:

- A Postman collection file with test cases.
- Assertions for HTTP status codes and response validations.
- Instructions for running tests via Newman.
- (Optional) HTML report generation.

---

## 📂 Files in This Repo

| File/Folder                                | Description                             |
|--------------------------------------------|-----------------------------------------|
| `api test collection.postman_collection.json` | Postman collection with test cases     |
| `newman-run-report.html` *(optional)*       | Auto-generated HTML report from Newman |
| `README.md`                                 | Project documentation                   |
| `*.png`                                     | Screenshots (Postman UI) *(optional)*  |

---

## 🧪 What This Collection Tests

- ✅ GET `/posts` returns status code `200 OK`
- ✅ Response is a JSON array
- ✅ Each object contains keys: `userId`, `id`, `title`, `body`
- ✅ Number of records and sample content validation

---

## 🚀 How to Run the Tests

### 1. ✅ Install Newman (if not already installed)

```bash
npm install -g newman
newman run "api test collection.postman_collection.json"
