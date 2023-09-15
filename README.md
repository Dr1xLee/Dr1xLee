import turtle
import random

# Создаем экран и черепаху
screen = turtle.Screen()
t = turtle.Turtle()

# Устанавливаем скорость рисования черепахи
t.speed(0)

# Устанавливаем цвет фона
screen.bgcolor("black")

# Устанавливаем палитру цветов
colors = ["red", "orange", "yellow", "green", "blue", "purple", "white"]

# Функция для рисования круга
def draw_circle(size):
    t.color(random.choice(colors))
    t.begin_fill()
    t.circle(size)
    t.end_fill()

# Настройки черепахи
t.penup()
t.goto(0, -200)
t.pendown()

# Рисуем абстрактный рисунок
for _ in range(72):
    draw_circle(100)
    t.right(5)

# Завершаем работу по клику на экран
screen.exitonclick()
