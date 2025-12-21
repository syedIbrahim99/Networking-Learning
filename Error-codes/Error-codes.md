

---

# 🌐 HTTP Status Codes – Super Simple & Real-Time

### 🧠 Base idea (one line)

**Browser asks → Server replies with a number (status code)**

---

## 🔵 INFORMATIONAL (100–199)

👉 *“I heard you, keep going”*

---

### **100 – Continue**

📌 **Meaning:**
Server says: *“I got the header, send the body now.”*

🧑‍💻 Real example:
Uploading a **big file** (video) to a server.

🧾 Story:
You knock on the door → owner says “Yes, come in” → then you enter fully.

```
Client  --->  "Can I send data?"
Server  --->  100 Continue
Client  --->  Sends full data
```

---

### **101 – Switching Protocols**

📌 **Meaning:**
Server agrees to change the protocol.

🧑‍💻 Real example:
HTTP → WebSocket (used in chat apps, live updates)

```
Client  --->  Request HTTP → WebSocket
Server  --->  101 Switching Protocols
Connection becomes WebSocket
```

---

## 🟢 SUCCESS (200–299)

👉 *“Everything is OK”*

---

### **200 – OK**

📌 **Meaning:**
Request successful.

🧑‍💻 Real example:
Opening **google.com**

```
Browser ---> Request page
Server  ---> 200 OK + Page data
```

---

### **201 – Created**

📌 **Meaning:**
Something **new is created** successfully.

🧑‍💻 Real example:
Creating a **new user account** or **new record**

```
Client ---> Create new user
Server ---> 201 Created (User created)
```

---

### **204 – No Content**

📌 **Meaning:**
Request successful, **but nothing to show back**.

🧑‍💻 Real example:
Deleting a record.

```
Client ---> Delete user
Server ---> 204 No Content
```

(No page, no message – just success)

---

## 🟡 REDIRECTION (300–399)

👉 *“Go somewhere else”*

---

### **301 – Moved Permanently**

📌 **Meaning:**
URL changed **forever**.

🧑‍💻 Real example:
`http://site.com` → `https://site.com`

```
Browser ---> Old URL
Server  ---> 301 → New URL
Browser ---> New URL
```

---

### **302 – Found (Temporary Move)**

📌 **Meaning:**
URL changed **temporarily**.

🧑‍💻 Real example:
Login redirect.

```
Browser ---> /login
Server  ---> 302 → /dashboard
```

---

### **304 – Not Modified**

📌 **Meaning:**
Use **cached data**, no need to download again.

🧑‍💻 Real example:
Reloading a website without changes.

```
Browser ---> Do you have new data?
Server  ---> 304 Not Modified
Browser ---> Uses cached version
```

---

## 🔴 CLIENT ERROR (400–499)

👉 *“Problem from your side (user/browser)”*

---

### **400 – Bad Request**

📌 **Meaning:**
Request is **wrong or broken**.

🧑‍💻 Real example:
Sending invalid JSON or missing fields.

```
Client ---> Wrong request format
Server ---> 400 Bad Request
```

---

### **401 – Unauthorized**

📌 **Meaning:**
Authentication **not provided or wrong**.

🧑‍💻 Real example:
Accessing API **without token**.

```
Client ---> Request without login
Server ---> 401 Unauthorized
```

---

### **403 – Forbidden**

📌 **Meaning:**
You are logged in, **but no permission**.

🧑‍💻 Real example:
Normal user trying to access **admin page**.

```
Client ---> Access admin page
Server ---> 403 Forbidden
```

---

### **404 – Not Found**

📌 **Meaning:**
Resource does **not exist**.

🧑‍💻 Real example:
Wrong URL.

```
Browser ---> /wrongpage
Server  ---> 404 Not Found
```

---

## 🔥 SERVER ERROR (500–599)

👉 *“Problem from server side”*

---

### **500 – Internal Server Error**

📌 **Meaning:**
Server crashed or code error.

🧑‍💻 Real example:
Null pointer, DB error, app crash.

```
Client ---> Valid request
Server ---> 500 Error (Something broke)
```

---

### **501 – Not Implemented**

📌 **Meaning:**
Server **doesn’t support** this request.

🧑‍💻 Real example:
Calling an API method not built yet.

```
Client ---> Feature request
Server ---> 501 Not Implemented
```

---

### **502 – Bad Gateway**

📌 **Meaning:**
Server got **bad response from another server**.

🧑‍💻 Real example:
Nginx → App server down.

```
Client ---> Nginx
Nginx  ---> App Server (Bad response)
Client <--- 502 Bad Gateway
```

---

### **503 – Service Unavailable**

📌 **Meaning:**
Server is **down or overloaded**.

🧑‍💻 Real example:
Server under maintenance.

```
Client ---> Request
Server ---> 503 Service Unavailable
```

---

### **504 – Gateway Timeout**

📌 **Meaning:**
Server **waited too long** for response.

🧑‍💻 Real example:
Slow database or API timeout.

```
Client ---> Nginx
Nginx  ---> Backend (No response)
Client <--- 504 Gateway Timeout
```

---

## 🧠 EASY MEMORY TRICK

| Range | Meaning         |
| ----- | --------------- |
| 1xx   | Wait / Continue |
| 2xx   | Success         |
| 3xx   | Redirect        |
| 4xx   | Your mistake    |
| 5xx   | Server mistake  |

---

