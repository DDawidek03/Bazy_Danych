# 🐍 Kurs Python

## 📄 Spis Treści

- 📖 [Wprowadzenie](#wprowadzenie)
- 🔢 [Typy Danych](#typy-danych)
- 🔁 [Struktury Kontrolne](#struktury-kontrolne)
  - ⛓️‍💥 [Łańcuchy Znaków](#łańcuchy-znaków)
  - 📜 [Instrukcje Warunkowe](#instrukcje-warunkowe)
  - 🔄 [Pętle](#pętle)
  - 📋 [Listy, tablice i słowniki](#listy-tablice-i-słowniki)
- 📦 [Moduły i Pakiety](#moduły-i-pakiety)
- 🗃️ [Praca z Plikami](#praca-z-plikami)
- 🧰 [Funkcje](#funkcje)
- 🚀 [Programowanie Obiektowe](#programowanie-obiektowe)
- 📊 [Matplotlib](#matplotlib)
- 🖼️ [Tkinter](#tkinter)
- 🐼 [Biblioteka Pandas](#biblioteka-pandas)
- 🔍 [Debugowanie i Testowanie](#debugowanie-i-testowanie)

## Wprowadzenie

Python to wszechstronny i popularny język programowania, znany ze swojej prostoty i czytelności. Umożliwia szybkie i efektywne tworzenie aplikacji, od skryptów automatyzujących codzienne zadania po złożone systemy i aplikacje webowe. Python jest językiem wysokiego poziomu, co oznacza, że skupia się na czytelności i prostocie składni, co ułatwia programowanie i zrozumienie kodu. Język Python ma bogatą bibliotekę standardową, która zawiera wiele gotowych modułów i funkcji.

## Typy Danych

Python jest dynamicznie typowanym językiem, co oznacza, że typ zmiennej jest określany automatycznie w czasie wykonywania programu. Oto tabela przedstawiająca niektóre z najpopularniejszych typów danych w Pythonie:

| Typ Danych  | Opis                                                                            | Przykład                                       |
| ----------- | ------------------------------------------------------------------------------- | ---------------------------------------------- |
| `int`       | Reprezentuje liczby całkowite.                                                  | `x = 42`                                       |
| `float`     | Reprezentuje liczby zmiennoprzecinkowe.                                         | `pi = 3.14`                                    |
| `str`       | Reprezentuje ciągi znaków.                                                      | `message = "Hello, World!"`                    |
| `bool`      | Reprezentuje wartości logiczne (TRUE/FALSE).                                    | `is_true = True`                               |
| `list`      | Reprezentuje uporządkowaną kolekcję elementów.                                  | `numbers = [1, 2, 3]`                          |
| `tuple`     | Reprezentuje uporządkowaną kolekcję elementów, które nie mogą być modyfikowane. | `coordinates = (1, 2, 3)`                      |
| `dict`      | Reprezentuje kolekcję par klucz-wartość.                                        | `person = {"name": "John", "age": 30}`         |
| `set`       | Reprezentuje kolekcję unikalnych elementów.                                     | `unique_numbers = {1, 2, 3}`                   |
| `datetime`  | Reprezentuje datę i czas.                                                       | `current_time = datetime.datetime(2022, 1, 1)` |
| `bytes`     | Reprezentuje sekwencję bajtów.                                                  | `data = b"Hello"`                              |
| `bytearray` | Reprezentuje modyfikowalną sekwencję bajtów.                                    | `mutable_data = bytearray(b"Hello")`           |
| `None`      | Reprezentuje brak wartości.                                                     | `value = None`                                 |
| `complex`   | Reprezentuje liczby zespolone.                                                  | `z = 3 + 4j`                                   |

### **Konwencje nazewnictwa zmiennych**

W Pythonie obowiązują pewne zasady i konwencje nazewnictwa zmiennych:

- Zmienne mogą zaczynać się od litery lub podkreślenia (\_), ale nie od cyfry.
- Mogą zawierać litery, cyfry i podkreślenia.
- Python rozróżnia wielkość liter, więc name i Name to dwie różne zmienne.
- Stosowanie konwencji snake_case do nazewnictwa zmiennych (np. user_name, total_amount).

Tworzenie zmiennej w języku Python zaczyna się od podania nazwy zmiennej, po której następuje znak równości = oraz przypisana wartość.

```python
zmienna_nazwa = 1
```

Opcjonalnie, na początku można dodać nazwę typu danych, aby kod był bardziej przejrzysty i czytelny

```python
int zmienna_nazwa = 1
```

## Struktury Kontrolne

Struktury kontrolne w Pythonie pozwalają na sterowanie przepływem wykonania programu. Umożliwiają one podejmowanie decyzji, powtarzanie bloków kodu i wykonywanie różnych operacji w zależności od określonych warunków.

## Łańcuchy Znaków

## Instrukcje Warunkowe

Instrukcje warunkowe pozwalają na wykonywanie różnych bloków kodu w zależności od warunków logicznych.

## Operatory logiczne i porównania

Operatory logiczne i porównania są używane do tworzenia warunków w instrukcjach warunkowych.

| Operator | Nazwa              | Przykład         | Opis                                                  |
| -------- | ------------------ | ---------------- | ----------------------------------------------------- |
| ==       | Równość            | x == y           | Sprawdza, czy x jest równe y                          |
| !=       | Nierówność         | x != y           | Sprawdza, czy x nie jest równe y                      |
| >        | Większe            | x > y            | Sprawdza, czy x jest większe od y                     |
| <        | Mniejsze           | x < y            | Sprawdza, czy x jest mniejsze od y                    |
| >=       | Większe lub równe  | x >= y           | Sprawdza, czy x jest większe lub równe y              |
| <=       | Mniejsze lub równe | x <= y           | Sprawdza, czy x jest mniejsze lub równe y             |
| and      | I                  | x > 0 and x < 10 | Sprawdza, czy oba warunki są prawdziwe                |
| or       | Lub                | x < 0 or x > 10  | Sprawdza, czy którykolwiek warunek jest prawdziwy     |
| not      | Negacja            | not x == y       | Neguje warunek, zmieniając True na False i vice versa |

### Instrukcja `if`:

Instrukcja `if` sprawdza, czy warunek jest prawdziwy, i jeśli tak, wykonuje blok kodu.

```python
x = 10

if x > 5:
    print(" x jest wieksze od 5")
```

### Instrukcja `if else`

Instrukcja `if`...`else` pozwala na wykonanie alternatywnego bloku kodu, jeśli warunek jest fałszywy.

```python
x = 3

if x > 5:
    print(" x jest wieksze od 5")
else:
    print("x jest mniejsze lub równe 5")
```

### Instrukcja `if elif else`

Instrukcja `if`...`elif`...`else` pozwala na sprawdzenie wielu warunków po kolei.

```python
x = 5
if x > 5:
    print("x jest większe od 5")
elif x == 5:
    print("x jest równe 5")
else:
    print("x jest mniejsze od 5")
```

## Pętle

## Listy, tablice i słowniki
