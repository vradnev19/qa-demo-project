# 🐞 BUG Report: Login allows empty password

**ID:** BUG-001  
**Module:** Login Form  
**Severity:** High  
**Priority:** High  

---

### Steps to Reproduce
1. Отвори Login страницата
2. Въведи валиден email (user@example.com)
3. Остави полето Password празно
4. Натисни "Login"

---

### Expected Result
- Системата не позволява вход
- Показва се грешка "Password is required"

---

### Actual Result
- Системата позволява вход с празна парола
- Потребителят попада в Dashboard

---

### Status
Open
