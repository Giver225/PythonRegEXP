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

![image](https://user-images.githubusercontent.com/85654567/173178848-5419b181-edba-4ea2-862f-47dedc759880.png)
![image](https://user-images.githubusercontent.com/85654567/173178880-763c8213-c572-4e52-ace9-ad0c13eac4db.png)
