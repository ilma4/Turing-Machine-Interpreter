## Ключевые слова

* Alphabet
* ExtraAlphabet
* States
* Function
* Success
* Fail
* Start
* Blank
* left
* right
* stay


## Комментарии

Коментарии реализованы как в C++, двух типов: однострочные, после ```//```, и многострочные, между ```/* */```.


## Идентефикаторы

Идентификатор сивола - строка из латинских букв(строчных и заглавных) и цифр, начинающаяся со строчного латинского символа.

Аналогично идентификатор состояния - строка из латинских букв(строчных и заглавных) и цифр, начинающаяся с заглавного латинского символа.

Примеры:

`char char1 abacaba` - символы

`State1 Bad Good` - состояния

## Переходы

Переход начинается с открывающей круглой скобки. Далее идут идентификаторы состояния и символа, разделённые пробельными символами, далее идёт "оператор" ```->```, после которого идут состояния, символ, одно из трёх ключевых слов: `left`, ```right``` или ```stay``` и закрывающая круглая скобка.

Примеры:

`(State1 char1 -> State2 char2 right)`

## Последовательности идентификаторов

Последовательность начинается с открывающей фигурной скобки ```{```. Далее идут идентификаторы одного типа(символ, состояние, переход), разделённые пробельными символами и/или переносами строк. Завершается последовательность закрывающей фигурной скобкой.

## Описание алфавитов и состояний

Алфавит и расширенный алфавит - последовательности сиволов, перед открывающей фигурной скобкой которых стоят ключевые слова `Alphabet` и `ExtraAlphabet` соответсвенно(без пробелов).

Аналогично состояния - последовательность состояний, перед которой стоит ключевое слово `States`.

Аналогично функция перехода - последовательность переходов, перед которой стоит ключевое слово `Function`.


## Допускающие/отвергающие состояния, пробельные сим.

Аналогично описываются допускающие(`Success`) и отвергающие(`Fail`) состояния, пробельный символ(`Blank`), начальное состояние(`Start`) 
