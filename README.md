string = input()
i = 0
amountOfSymbl = 1
for i in range(0, len(string) - 1):
    if string[i] == string[i + 1]:
        amountOfSymbl += 1
    else:
        print('{}{}'.format(string[i], amountOfSymbl), end='')
        amountOfSymbl = 1
print('{}{}'.format(string[i + 1], amountOfSymbl))
