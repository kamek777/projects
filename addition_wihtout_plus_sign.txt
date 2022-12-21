# funckja sumująca dwie liczby bez znaku "+"
def dodawanie_bez_znaku_plus(a, b):
    while b!=0:
        zbior = a & b
        a = a^b
        b = zbior << 1
    return a
### przykład użycia:
print("10+24=",dodawanie_bez_znaku_plus(10,24))
print("0+12=",dodawanie_bez_znaku_plus(0,12))