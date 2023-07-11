limit = int(input("Введите число: "))
prime_numbers = []
for num in range(2, limit + 1):
    is_prime = True
    for i in range(2, num):
        if num % i == 0:
            is_prime = False
            break
    if is_prime:
        prime_numbers.append(num)
print("Простые числа до", limit, ":", prime_numbers)
