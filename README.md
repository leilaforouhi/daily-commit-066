def gcd(a, b):
    while b != 0:
        a, b = b, a % b
    return a

def lcm(a, b):
    return abs(a * b) // gcd(a, b)

if __name__ == "__main__":
    x = 12
    y = 15
    print(f"LCM of {x} and {y} is {lcm(x, y)}")
