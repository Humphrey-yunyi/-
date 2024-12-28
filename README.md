# -
测试
def is_prime(n):
    if n <= 1:
        return False
    if n == 2:
        return True
    if n % 2 == 0:
        return False
    for i in range(3, int(n**0.5) + 1, 2):
        if n % i == 0:
            return False
    return True

# 示例使用
number = 29
if is_prime(number):
    print(f"{number} 是质数")
else:
    print(f"{number} 不是质数")
