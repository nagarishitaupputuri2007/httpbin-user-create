# 👩‍💻 HTTPBin User Creation API Testing

## 🧩 Overview
This assignment tests the **user creation API** of a hiring platform using the HTTPBin service.  
The goal is to verify **POST request behavior**, ensure correct **JSON handling**, and observe **echoed responses**.

---

## 🔗 API Endpoint
`POST → https://httpbin.org/post`

---

## 🧪 Testing Setup

- **Tool Used:** Postman  
- **Request Type:** POST  
- **Header:** `Content-Type: application/json`  
- **Body Format:** JSON  

---

## 📋 Test Data Used

| Request # | Name | Job |
|------------|------|-----|
| 1 | Alice Johnson | Frontend Developer |
| 2 | Bob Williams | Backend Engineer |
| 3 | Naga Rishita Upputuri | Data Analyst Intern |

---

## 📤 Observed Responses

Each response included:
- ✅ `json` → Echoed back name & job data  
- ✅ `headers` → Metadata including content type  
- ✅ `origin` → Client IP  
- ✅ `status` → 200 OK  

---

## 🧱 One Sample Request/Response Example

### **Request**
```http
POST https://httpbin.org/post
Content-Type: application/json

{
  "name": "Naga Rishita Upputuri",
  "job": "Data Analyst Intern"
}
```

### **Response**
```json
{
  "url": "https://httpbin.org/post",
  "json": {"name": "Naga Rishita Upputuri", "job": "Data Analyst Intern"},
  "headers": {"Content-Type": "application/json"},
  "origin": "192.168.1.12",
  "status": 200
}
```

---

## 🧱 Technologies Used
- Postman (for API testing)  
- HTTPBin.org (for request/response simulation)  
- JSON (for structured data storage)

---

## 🧾 Submission Details
**GitHub Repo:** [https://github.com/nagarishitaupputuri2007/httpbin-user-create](https://github.com/nagarishitaupputuri2007/httpbin-user-create)  
**Created On:** 2025-11-12 08:44:53

---

## ✅ Notes
- This API does not persist user data — it only echoes your request.
- Each POST request was independent and returned the expected structure.
