# HW_18
# Запрос количества билетов
num_tickets = int(input("Сколько билетов вы хотите купить? "))

# Инициализация общей стоимости заказа
total_cost = 0

# Подсчет стоимости каждого билета
for _ in range(num_tickets):
    age = int(input("Введите возраст посетителя: "))
    
    if age < 18:
        total_cost += 0
    elif 18 <= age < 25:
        total_cost += 990
    else:
        total_cost += 1390

# Проверка на скидку
if num_tickets > 3:
    total_cost *= 0.9  # Применение 10% скидки

# Вывод общей стоимости к оплате
print("Итого к оплате:", total_cost, "рублей")
