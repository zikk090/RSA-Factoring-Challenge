import sys

def factorize(num):
    """
    Factorize a number into a product of two smaller numbers.
    """
    for i in range(2, num):
        if num % i == 0:
            return i, num // i
    return None

if __name__ == '__main__':
    if len(sys.argv) != 2:
        print('Error: More than one argument')
        sys.exit(1)

    file_path = sys.argv[1]
    with open(file_path, 'r') as f:
        for line in f:
            num = int(line[:-1])
            factors = factorize(num)
            if factors:
                print(f'{num}={factors[0]}*{factors[1]}')

