
### Формулировка
Напишите программу для определения сезона года по номеру месяца.

### Пояснение
Программа должна принимать на вход номер месяца и выводить соответствующий сезон года. Например, для месяцев с декабря по февраль включительно выводится "зима", для месяцев с марта по май - "весна" и так далее.

### Тесты

1. **Пример 1:**
   - Вход: `month = 12`
   - Ожидаемый вывод: `"зима"`

2. **Пример 2:**
   - Вход: `month = 4`
   - Ожидаемый вывод: `"весна"`

3. **Пример 3:**
   - Вход: `month = 9`
   - Ожидаемый вывод: `"осень"`

### JavaScript
```javascript
function seasonByMonth(month) {
    if (month === 12 || month === 1 || month === 2) {
        return "зима";
    } else if (month >= 3 && month <= 5) {
        return "весна";
    } else if (month >= 6 && month <= 8) {
        return "лето";
    } else if (month >= 9 && month <= 11) {
        return "осень";
    } else {
        return "Ошибка: введен некорректный номер месяца.";
    }
}
```
