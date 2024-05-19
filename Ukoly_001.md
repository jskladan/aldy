# Deleni ukolu na mensi casti

Vyber si nekolik "beznych cinnosti" (vyper pradlo, jdi na nakup, uvar polevku), a rozepis je v ruzne urovni detailu jako algoritmus.

# Programovani

## Program 1

* Vytvor promennou `x` a nastavi ji na cele cislo
* Do promenne `s` prirad retezec "Hello World!"
* Promennou `aldy` nastav na slovnik s klici jmeno, prijmeni a adresa. Jmeno a prijmeni budou retezce, adresa bude slovnik s klici ulice a mesto
* Vytvor pole celych cisel 10-20 a uloz ho do promenne jmenem `cisla`
* Promennou `bydliste` nastav hodnotu `adresa` ze slovniku `aldy`

Vypis na vystup:
 * posledni znak retezce v promenne `s`
 * druhy, paty a osmy prvek pole `cisla`
 * jmeno ulice, na ktere bydli `aldy`


## Program 2

* Vytvor promennou jmenem `hesla` uloz do ni pole peti "nahodnych" retezcu (slov)
* Do promenne `x` nacti vstup od uzivatele
* Do promenne `y` nacti vstup od uzivatele
* Pokud je `x` rovno prvnimu prvku pole `hesla` a soucasne `y` se nerovna poslednimu prvku, vypis "OK", jinak vypis "NOPE!"


## Program 3

Zkopiruj kod Programu 2, prepis ho tak, aby splnoval nasledujici:
 * Pokud jsou oba vstupy "spravne" vypis "OK"
 * Pokud je chybna hodnota `x` vypis "Spatna prvni cast hesla"
 * Pokud je chybna hodnota `y` vypis "Spatna druha cast hesla"
 * Pokud jsou spatne oba vstupy, vypis "NOPE!"


## Program 4

* Nacti vstup od uzivatele do promenne `v`
* Pokud vstup obsahuje alespon dve slova, vypis "OK", jinak vypi "NOPE!"

Hint:
 * https://docs.python.org/3/library/stdtypes.html#str.split
 * https://docs.python.org/3/library/functions.html#len

## Bonus 1

* Nacti od uzivatele vstup do promenne `v`
* Rozdel `v` na jednotliva slova (pro zjednoduseni predpokladej, ze na zacatku ani na konci vstupu neni mezera) a toto pole slov uloz do promenne `slova`
* Vypis na vystup pouze nejdelsi slovo (pro zjednoduseni predpokladej, ze existuje prave jedno nejdelsi slovo)

## Bonus 2

* U programu Bonus 1 se zamysli, jak bys rozpoznal (a pripadne resil) situaci, kdy vstup obsahuje vic nez jedno "nejdelsi" slovo.
