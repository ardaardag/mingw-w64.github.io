#include <iostream>

int main()
{

    double sayi1, sayi2;
    char islem;
    std::cout << "birinci sayıyı gir:";
    std::cin >> sayi1;

    std::cout << "ikinci sayıyı gir:";
    std::cin >> sayi2;

    std::cout << "yapmak istediğin işlemi gir (+,-,*,/):";
    std::cin >> islem;


    double sonuç;


    if (islem == '+') {
        sonuç = sayi1 + sayi2;

    }
    else if (islem == '-') {
        sonuç = sayi1 - sayi2;
    }
    else if (islem == '*') {
        sonuç = sayi1 * sayi2;
    }
    else if (islem == '/') {
        if (sayi2 != 0)
            sonuç = sayi1 / sayi2;


        else {
            std::cout << "Hata: sıfıra bölünmez!" << std::endl;

            return 0;

        }
    }
    else {
        std::cout << "Geçersiz işlem sembolü girdiniz!" << std::endl;
        return 0;

    }
    std::cout << "sonuc:" << sonuç << std::endl;
    return 0;

}
