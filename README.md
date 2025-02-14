## Висновки щодо точності методу Монте-Карло для обчислення інтегралів

### Опис проблеми
Метою цього завдання було обчислити значення визначеного інтегралу для функції y = x^3 на інтервалі [0, 1] за допомогою методу Монте-Карло та перевірити результат за допомогою точного методу — функції quad з бібліотеки SciPy.

### Результати
- Метод Монте-Карло: Отримане значення інтегралу змінюється залежно від кількості точок, використаних для оцінки. Наприклад, для 100000 вибірок результат був близьким до точного аналітичного значення.
- Функція `quad`: Це метод з високою точністю, який використовує чисельні методи для точного обчислення визначених інтегралів. Для нашої функції результат становив близько 0.25.

### Порівняння
- **Метод Монте-Карло**: дає точність, яка залежить від кількості вибірок. Чим більше вибірок, тим точніший результат. Для 100000 вибірок ми отримали значення дуже близьке до 0.25 (аналітичного розрахунку).
- **Метод quad**: дає точне значення інтегралу, яке є референтним для порівняння з методом Монте-Карло.

### Висновок
Метод Монте-Карло є корисним для випадків, коли неможливо аналітично обчислити інтеграл, або для інтегралів з багатьма змінними. Проте його точність залежить від кількості вибірок, і для складних функцій або високих вимог до точності необхідно використовувати достатньо вибірок. Для задачі на обмеженому інтервалі, як у нашому прикладі, метод Монте-Карло дає близькі результати до аналітичних значень при великій кількості вибірок.
