import random
import string

def generate_password(length):
    letters = string.ascii_lowercase + string.digits + "!@#$%^&*"   
    password = random.choice(letters)
    for i in range(length -1):
        password += random.choice(letters)
    print('вот ваш пароль:',password)

def check_password_strength(password):
    if len(password) < 8:
        if password.isalpha() or password.isdigit():
            print('Ваш пароль небезопасен!')
        else:
            print('Ваш пароль слабый')
    elif password.isalnum():
        print('Ваш пароль средний')
    else:
        print('Ваш пароль очень хороший')

def main():
    glavnoe = input('введите generate если хотите сгенерировать пароль или check что бы проверить ваш пороль:')
    if glavnoe == 'generate':
        length = int(input('введите длину пароля:'))
        generate_password(length)
    elif glavnoe == 'check':
        password = input('Введите пароль для проверки защиты:')
        check_password_strength(password)
    else:
        print('вы ввели не то попробуйте еще раз')

main()
