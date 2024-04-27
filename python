import itertools

def generate_strings():
    # Generate combinations of digits and lowercase letters
    combinations = itertools.product(range(10), repeat=4)  # 0000 to 9999
    letters = 'abcdefghijklmnopqrstuvwxyz'
    for combo in combinations:
        for letter_combo in itertools.product(letters, repeat=6):  # aaaaaa to zzzzzz
            yield ''.join(str(x) for x in combo) + ''.join(letter_combo)

def save_strings_to_file():
    with open('output.txt', 'w') as file:
        for i, string in enumerate(generate_strings()):
            file.write(string + '\n')

save_strings_to_file()
