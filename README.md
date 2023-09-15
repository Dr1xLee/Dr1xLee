- 👋 Hi, I’m @Dr1xLee
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Dr1xLee/Dr1xLee is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
# Функция для сложения
def add(x, y):
    return x + y

# Функция для вычитания
def subtract(x, y):
    return x - y

# Функция для умножения
def multiply(x, y):
    return x * y

# Функция для деления
def divide(x, y):
    if y == 0:
        return "Деление на ноль невозможно"
    return x / y

# Основной код программы
while True:
    print("Выберите операцию:")
    print("1. Сложение")
    print("2. Вычитание")
    print("3. Умножение")
    print("4. Деление")
    print("5. Выход")

    choice = input("Введите номер операции (1/2/3/4/5): ")

    if choice == '5':
        print("Программа завершена.")
        break

    if choice not in ('1', '2', '3', '4'):
        print("Некорректный ввод. Попробуйте еще раз.")
        continue

    num1 = float(input("Введите первое число: "))
    num2 = float(input("Введите второе число: "))

    if choice == '1':
        print("Результат:", add(num1, num2))
    elif choice == '2':
        print("Результат:", subtract(num1, num2))
    elif choice == '3':
        print("Результат:", multiply(num1, num2))
    elif choice == '4':
        print("Результат:", divide(num1, num2))
