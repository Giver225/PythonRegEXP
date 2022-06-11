# PythonRegEXP
import math


def main(z, x, y):
    n = len(x)
    s = 0
    x.insert(0, 0)
    y.insert(0, 0)
    z.insert(0, 0)
    for i in range(1, n + 1):
        s += (3 * z[math.ceil(i / 4)] ** 2 + y[math.ceil(i / 2)] +
              28 * x[n + 1 - math.ceil(i / 3)] ** 3) ** 6 / 96
    return s
ИЛИ СМОТРИ ФАЙЛ В ЭТОМ РЕПОЗИТОРИИ

![image](https://user-images.githubusercontent.com/85654567/173178848-5419b181-edba-4ea2-862f-47dedc759880.png)

def main(x):
    a = 0x7f
    b = 0x7f << 7
    c = 0xf << 14
    d = 0x7ff << 18
    e = 0x7 << 29

    e = (e & x) >> 29
    d = (d & x) >> 4
    c = (c & x) >> 11
    b = (b & x) << 18
    a = (a & x) << 7
    return c | b | a | d | e

![image](https://user-images.githubusercontent.com/85654567/173178880-763c8213-c572-4e52-ace9-ad0c13eac4db.png)
