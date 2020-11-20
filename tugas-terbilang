#satuan
#belasan
#puluhan
#ratusan
#jutaan
#miliyar

# 2 = dua = satuan
# 12 = dua belas = belasan
# 26 = dua puluh enam = puluhan
# 267 = dua ratus enam puluh tujuh = ratusan
# 2672 = dua ribu enam ratus tujuh puluh dua = ribuan
# 200000 = dua juta = jutaan
# 200000000 = dua miliyar = miliyar

kata = ['','one','two','three','four','five','six','seven','eight','nine']

def terbilang(n):
    global terbilang

    if n < 10:
        return kata[n]
    elif n >= 1_000_000_000:
        return terbilang(n // 1_000_000_000) + ' billion ' + (terbilang(n % 1_000_000_000) if n % 1_000_000 != 0 else '')
    elif n >= 1_000_000:
        return terbilang(n // 1_000_000) + ' million ' + (terbilang(n % 1_000_000) if n % 1_000_000 != 0 else '')
    elif n >= 1_000:
        if n // 1_000 == 1:
            return " one thousand " + (terbilang(n % 1_000) if n % 1_000 != 0 else '')
        else:
            return terbilang(n // 1_000) + " thousand " + (terbilang(n % 1_000) if n % 1_000 != 0 else '')
    elif n >= 100:
        if n // 100 == 1:
            return ' one hundred ' + (terbilang(n % 100) if n % 100 != 0 else '')
        else:
            return terbilang(n // 100) + ' hundred ' + (terbilang(n % 100) if n % 100 != 0 else '')
    elif n >= 20:
        if n == 21:
            return 'twenty one'
        if n == 22:
            return 'twenty two'
        if n == 23:
            return 'twenty three'
        if n == 24:
            return 'twenty four'
        if n == 25:
            return 'twenty five'
        if n == 26:
            return 'twenty six'
        if n == 27:
            return 'twenty seven'
        if n == 28:
            return 'twenty eight'
        if n == 29:
            return 'twenty nine'
        if n == 30:
            return 'thirty'
        if n == 50:
            return 'fifty'
        return terbilang (n//10) + 'ty' + (terbilang(n % 10) if n % 10 !=0 else'')
    else:
        if n == 10:
            return 'ten'
        elif n == 11:
            return 'eleven'
        elif n == 12:
            return 'twelve'
        elif n == 13:
            return 'thirteen'
        elif n == 15:
            return 'fifteen'
        else:
            return terbilang(n % 10) + 'teen'

#test
import os
while True:
    os.system('cls')
    try:
        n = int(input('angka?'))
        print (f'{n:,}={terbilang(n)}')
    except:
        print('data input anda tidak benar..')
    os.system('pause')
