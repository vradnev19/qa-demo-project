# Test Cases: Authentication (Login & Registration)

---

## ID: TC-003
**Title:** Логин с грешен имейл

**Preconditions:**
- Потребителят има валиден акаунт: user@example.com / password123

**Steps:**
1. Отвори Login страницата
2. Въведи грешен имейл: wrong@example.com
3. Въведи валидна парола: password123
4. Натисни "Login"

**Expected Result:**
- Появява се съобщение: "Invalid email or password"
- Входът е отказан

---

## ID: TC-004
**Title:** Логин с твърде кратка парола

**Steps:**
1. Отвори Login страницата
2. Въведи валиден имейл: user@example.com
3. Въведи парола: "12"
4. Натисни "Login"

**Expected Result:**
- Появява се съобщение: "Password must be at least 6 characters"
- Няма вход

---

## ID: TC-005
**Title:** Успешна регистрация с валидни данни

**Steps:**
1. Отвори Registration страницата
2. Въведи име: "Test User"
3. Въведи имейл: newuser@example.com
4. Въведи парола: password123
5. Потвърди парола: password123
6. Натисни "Register"

**Expected Result:**
- Потребителят се създава успешно
- Пренасочване към Login или Dashboard

---

## ID: TC-006
**Title:** Регистрация с вече използван имейл

**Steps:**
1. Отвори Registration страницата
2. Въведи име: "Test User"
3. Въведи имейл: user@example.com (вече съществуващ)
4. Въведи парола: password123
5. Потвърди парола: password123
6. Натисни "Register"

**Expected Result:**
- Появява се грешка: "Email is already taken"
- Регистрацията е отказана

---

## ID: TC-007
**Title:** Регистрация с различни пароли

**Steps:**
1. Отвори Registration страницата
2. Въведи име: "Test User"
3. Въведи имейл: testuser@example.com
4. Въведи парола: password123
5. Потвърди парола: password321
6. Натисни "Register"

**Expected Result:**
- Появява се грешка: "Passwords do not match"
- Няма създаден акаунт
