# Test Case: Login Form

## ID: TC-001
**Title:** Успешен логин с валидни данни

**Preconditions:**
- Потребителят има валиден акаунт (user@example.com / password123)

**Steps:**
1. Отвори Login страницата
2. Въведи валиден email
3. Въведи валидна парола
4. Натисни "Login"

**Expected Result:**
- Успешен вход → пренасочване към Dashboard
---

## ID: TC-002
**Title:** Неуспешен логин с празна парола

**Steps:**
1. Отвори Login страницата
2. Въведи валиден email
3. Остави паролата празна
4. Натисни "Login"

**Expected Result:**
- Показва се съобщение: "Password is required"
- Няма вход в системата
