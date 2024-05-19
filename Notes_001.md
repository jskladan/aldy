# Termity a tak

## Zakladni datove typy

Je toho vic, toto pro zacatek staci:

 * `int` (integer) - cela cisla
 * `float` - desetinna cisla
 * `str` (string) - retezce (~~ posloupnosti/pole znaku)
 * `list` - pole/seznam (usporadana kolekce hodnot libovolneho typu)
 * `dict` (dictionary) - slovnik (mapuje klice na hodnoty)
 * `bool` (boolean) - pravda/nepravda (nabyva jen hodnoty `True` nebo `False`)

Pole a slovniky do sebe jdou libovolne zanorovat.

https://docs.python.org/3.3/library/stdtypes.html


## Zakladni stavebni prvky programu

Opet bare-bones:

 * promenna (variable) - symbolicke jmeno/idenfitikator mista v pameti, do promennych se prirazuji hodnoty
 * podminka (`if-elif-else`)
    * zakladni porovnani
        * rovnost: `1 == 1`
        * nerovnost: `1 != 2`
        * vetsi/mensi: `2 > 3`, `4 < 5`
        * pole obsahuje prvek: `1 in [1,2,3,4]`
        * retezec neobsahuje obsahuje "text": `"ep" in "ahoj pepo"`

    * skladani podminek (boolean algebra)
        * `and` (oboji soucasne je pravda): `(1 < 2) and (3 == 9/3)`
        * `or` (jedna, druha, nebo obe soucasne): `(3 < 1) or (2 == 2) or (3 >= 4)`
        * `not` (negace): `not (4 in [1,2,3])`

 * cyklus
   * `for` - prochazi nejakou kolekci prvku od zacatku do konce (treba vsecky polozky listu)
   * `while` - vykonava telo cyklu se dokud plati podminka
 * funkce/procedura/metoda - pojmenovany "zaobaleny" blok kodu. Typicky prebira hodnoty (parametry) na vstupu, a generuje (`return`) navratovou hodnotu na vystupu
 * komentar - kus "kodu" ktery Python ignoruje. Typicky cokoli od znaku `#` do konce radku

https://docs.python.org/3/tutorial/controlflow.html


## Zakladni interakce s uzivatelem

* `input("Prompt: ")` - nacte vstup od uzivatele, a vrati jako navratovou hodnotu
* `print("Hodnota promenne je:", x)` - vypise na obrazovku hodnoty predane jako vstupni parametry


# Ukazky kodu

Vytvor promennou jmenem `heslo` s hodnotou `"foobar"`:

    heslo = "foobar"

Nacti vstup od uzivatele, uloz ho do promenne `x` a nezmeneny ho vypis na vystup:

    x = input("Zadej heslo: ")
    print(x)

Nacti vstup, pokud prvni znak na vstupu je `"A"` vypis `"OK"` (retezec je jakoby pole znaku):

    x = input("Zadej heslo: ")
    if x[0] == "A":
        print("OK")

Nacti vstup, pokud je stejny jako obsah promenne `heslo` vypis `"OK"`, jinak vypis `"NOPE!"`:

    heslo = "foobar"
    x = input("Zadej heslo: ")
    if x == heslo:
        print("OK")
    else:
        print("NOPE!")

---

Vytvor pole s hodnotami 1, 2, 3, 4, 5:

    p = [1, 2, 3, 4, 5]

Vypis prvni polozku pole na vystup:

    print(p[0])

Vypis druhou a treti polozku pole na vystup:

    print(p[1], p[2])

Vypis kazdou polozku z pole na vystup:

    for i in p:
        print(i)

Vypis kazdou sudou polozku z pole na vystup:

    for i in p:
        if i // 2 == 0: # // je celociselne deleni, tj 22/3 == 7.33333 ale 22//3 == 7
            print(i)

Nastav prvni polozku pole na hodnotu `"Zacatek"`:

    p[0] = "Zacatek"

Nastav posledni polozku pole na `"Konec"`:

    p[4] = "Konec"
    # Alternativne, Python umi "zaporne indexovani"
    p[-1] = "Konec"

---

Do promenne `joza` uloz slovnik, ktery bude klici a hodnotami popisovat jmeno, prijmeni a adresu:

    joza = {"jmeno": "Josef", "prijmeni": Skladanka, "adresa": "Rohacova 358, Kolin"}

Vypis na vystup jmeno a prijmeni z tohoto slovniku:

    print(joza["jmeno"], joza["prijmeni"])

Nastav adresu na slovnik s klici `"ulice"`, `"cislo"`, a `"mesto"`:

    joza["adresa"] = {"ulice": "Rohacova", "cislo": 358, "mesto": "Kolin"}

