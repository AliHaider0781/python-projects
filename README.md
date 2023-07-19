# python-projects
def fibonacci(max_num):
    fib_list = [0, 1]
    while True:
        next_fib = fib_list[-1] + fib_list[-2]
        if next_fib > max_num:
            break
        fib_list.append(next_fib)
    return fib_list

if __name__ == '__main__':
    max_num = int(input("Enter the maximum number for the sequence: "))
    fib_seq = fibonacci(max_num)
    print("The Fibonacci sequence up to {}:".format(max_num))
    print(fib_seq)
