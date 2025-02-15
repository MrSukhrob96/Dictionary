# Tushunchalar lug'ati havolalari bilan

Diqqat! Har bir mavzu bo'yicha videodarsga havolalar o'z repozitoriylarida joylashtirilgan.

Mundarija:
- [Boshlang'ich tushunchalar](https://github.com/HowProgrammingWorks/Dictionary#Базовые-понятия)
- [Asosiy tushunchalar](https://github.com/HowProgrammingWorks/Dictionary#Основные-понятия)
- [Yordamchi materiallar](https://github.com/HowProgrammingWorks/Dictionary#Вспомогательные-материалы)
- [Ma'lumotlar tuzilmalasi](https://github.com/HowProgrammingWorks/Dictionary#Структуры-данных)
- [Kengaytirilgan tushunchalar](https://github.com/HowProgrammingWorks/Dictionary#Расширенные-понятия)
- [Parallel dasturlash](https://github.com/HowProgrammingWorks/Dictionary#Параллельное-программирование)
- [Asinxron dasturlash](https://github.com/HowProgrammingWorks/Dictionary#Асинхронное-программирование)
- [Dasturlash paradigmalari](https://github.com/HowProgrammingWorks/Dictionary#Парадигмы-программирования)

## Boshlang'ich tushunchalar

- [Abstraktsiya / Abstraction](https://github.com/HowProgrammingWorks/Reusable)
mohiyatni ajratib ko'rsatgan holda muhim bo'lgan narsalarga urg'u berib va muhim bo'lmagan xususiyat va aloqalarni umumlashtirishdir. Abstraktsiyalash - abstraktsiyalar yoki modellarni qurish, algoritmlar va ma'lumotlar tuzilmalaridan qayta foydalanishni imkonini kuchaytiradi.
  - Abstraktsiya - bu muammoning umumlashtirilgan echimi (muayyan echimdan farqli o'laroq),
  keng ko'lamli vazifalar uchun moslangan;
  - Abstraktsiya - muammoni hal qilish uchun etarli bo'lgan haqiqiy ob'ekt modeli (ob'ektlar to'plami)ni haqiqatga yaqinlashtirgan holda umumlashtirish;
  - Abstraktsiya - ob'ektning ma'lum bir tomoni bilan bog'liq bo'lgan, muammoni hal qilish uchun zarur bo'lgan xususiyatlari va munosabatlarining to'plami;
  - [Abstraksiya qatlamlari / Abstraction Layer](https://github.com/HowProgrammingWorks/AbstractionLayers)
- Dasturlash paradigmalasi / Programming Paradigm
  - Paradigma g'oyalar va tushunchalar, ruhsatlar va cheklovlar, kontseptsiyalar, printsiplar, postulatlar, kompyuterda muammolarni hal qilish texnikasi va dasturlash usullarini belgilaydi;
  - Paradigma muammolarni echish uchun modelni, dastur kodini yozish uchun ishlatiladigan ma'lum bir uslubni, shablonlarni (yaxshi va yomon echimlarning misollarini) taklif qiladi;
- Sintaksis / Syntax - belgilardan dastur kodini tuzish qoidalari, lekin kodning mano (semantik) yuklanishiga ta'sir qilmaydi. Sintaksis faqat kodning rasmiy tuzilishini belgilaydi.
- Qiymat / Value - bu xotirada ma'lum bir joyga ma'lum formatda yozilgan va dastur tomonidan boshqariladigan ma'lumotlarni ifodalovchi qiymat.
- Tur / Type - bu qiymatlar bo'yicha bajarilishi mumkin bo'lgan qiymatlar va operatsiyalar to'plami. Masalan, JavaScript-da, `Boolean` turi ikkita qiymatni `true` va `false` va ular bo'yicha mantiqiy operatsiyalarni qabul qiladi, `Null` turi bitta `null` qiymatini oladi, `Number` turi esa minimal va maksimal qiymatlarga qo'shimcha cheklovlar hamda aniqlik bo'yicha cheklovlarga ega bo'lgan ratsional sonlar to'plami va matematik operatsiyalar `+ - * ** / % ++ -- > < >= <= & | ~ ^ << >>`.
  - [Ma'lumot turlari / Data Types](https://github.com/HowProgrammingWorks/DataTypes)
  - `[5, 'Tashkent', true, { city: 'Beijing' }, a => ++a ].map(x => typeof x);`
- Literal - dastur kodida qiymat yozish. Masalan: raqamlar, mantiqiy qiymatlar, null va undefined qatorlar, massivlar, ob'ektlar, funktsiyalar literallari.
Literallar turli xil sintaksislarga ega bo'lishi mumkin, raqamlarni yozish uchun juda oddiy sintaksisdan ob'ektlarni yozish uchun murakkab sintaksisgacha.
- Skalyar / Scalar / Primitive / Atomic value - primitiv ma'lumotlar turining qiymati.
Skalyar o'zlashtirilganda ko'chiriladi va funktsiyaga qiymati bo'yicha uzatiladi.
- Havola / Reference - havolali turidagi qiymatga ishora qiladi, yani skalyar bo'lmagan qiymatga, JavaScript uchun bu `Object, Function, Array`.
  - [havolali turlar](https://github.com/HowProgrammingWorks/DataTypes)
  - [massivlar va ob'ektlar bo'yicha kodga misollar](https://github.com/HowProgrammingWorks/DataStructures)
- Identifikator / Identifier - ichki va tashqi modullardan import qilingan va global o'zgaruvchilar, konstantalar, funktsiyalar, method-lar, argumentlar, class-lar nomlari.
- [O'zgaruvchi / Variable](https://github.com/HowProgrammingWorks/DataTypes) -
bu ma'lumot turi, manzili va qiymatiga ega bo'lgan nomlangan xotira maydoni (identifikator). O'zgaruvchining qiymatini konstantadan farqli o'laroq o'zgartirishimiz mumkin (va ba'zi tillar uchun esa turini ham): `let cityName = 'Tashkent';`
- Biriktirish / Assignment - qiymat va identifikatorni (masalan: o'zgaruvchi) bog'lash. Ko'pgina tillarda biriktirish jarayoni tayinlangan qiymatni qaytaradi (ifoda feliga ega).
- [Konstanta / Constant](https://github.com/HowProgrammingWorks/DataTypes) -
o'zgarmas qiymat va turga bog'langan identifikator:
`const WATCH_TIMEOUT = 5000;`
- [Strukturaviy turlar / Composed types](https://github.com/HowProgrammingWorks/DataTypes) -
kompozitsion turlar yoki tuzilmalar birlashtirilgan bir nechta skalyar qiymatlardan iborat bo'lib, shu kombinatsiyalangan qiymat bo'yicha bir qator operatsiyalar bajarilishi mumkin, masalan: obyekt, massiv, to'plam, kortej.
- [Sanaladigan turlar / Enumerated types](https://github.com/HowProgrammingWorks/Enum)
- Bayroq / Flag - Biror narsaning holatini belgilaydigan mantiqiy qiymat, masalan, ulanishni yopish belgisi, ma'lumotlar tarkibidagi qidiruvni yakunlash belgisi va boshqalar.
Masalan: `let flagName = false;` Ba'zan, mantiqiy emas, balki sanaladigan turlarni bayroqlar deb atash mumkin.
- Algoritm / Algorithm - bu cheklangan vaqt ichida ma'lum bir sinf muammolari uchun hisoblash tartibini rasmiy tavsifi (har qanday kirish ma'lumotlari to'plami uchun bajarish qobiliyati).
- Программа / Program - программный код и данные, объединенные в одно целое для
вычисления и управления ЭВМ.
- Инженерия / Engineering - извлечение практической пользы из имеющихся ресурсов
при помощи науки, техники, различных методик, организационной структуры, а так
же приемов и знаний.
- Инженерия программного обеспечения / Software engineering - приложение
инженерии к индустрии программного обеспечения. Включает архитектуру,
исследование, разработку, тестирование, развертывание и поддержку ПО.
- Программирование / Programming - это искусство и инженерия решения задач при
помощи вычислительной техники.
- Кодирование / Coding - написание исходного кода программы при помощи
определенного синтаксиса (языка), стиля и парадигмы по готовому ТЗ.
- Разработка программного обеспечения / Software development - это соединение
программирования и кодирования на всех этапов жизненного цикла ПО:
проектирования, разработки, тестирования, отладки, поддержки, сопровождения и
модификации.
- Инструкция / Instruction - один шаг алгоритма вычислений, например инструкция
процессора исполняется CPU.
- Оператор / Statement - наименьшая синтаксическая часть языка программирования,
исполняемая интерпретатором, средой или компилируемая в машинный код.
- Команда / Command - атомарная задача для командного процессора.
- Выражение / Expression - синтаксическая конструкция языка программирования
предназначенная для выполнения вычислений. Выражение состоит из идентификаторов,
значений, операторов и вызова функций. Пример: `(len - 1) * f(x, INTERVAL)`
- Блок кода / Block - логически связанная группа инструкций или операторов.
Блоки создают область видимости. Блоки могут быть вложенными. Примеры: `{}`,
`(+ a b)`, `begin end`, отступы в Python.
- Процедура или подпрограмма / Procedure or Subroutine - логически связанная
группа инструкций или операторов, имеющая имя. Процедура способствует повторному
использованию кода и может быть вызвана из разных частей программы, много раз
и с разными аргументами. Процедура не возвращает значений, в отличие от функций,
но в некоторых языках (но не в JavaScript) может модифицировать свои аргументы.
Во многих языках процедура описывается при помощи синтаксиса функций (например,
типа void).
- Функция / Function - абстракция преобразования значений. Функция однозначно
отображает одно множество значений в другое множество значений. Функция может
быть задана блоком операторов или выражением. Функция имеет набор аргументов.
Функция может быть вызвана по имени или через указатель. Функция способствует
повторному использованию кода и может быть вызвана из разных частей программы,
много раз и с разными аргументами. В JavaScript функция описывается при помощи
function или синтаксиса стрелок (лямбда-функций).
- Сигнатура функции / Function signature - имя (идентификатор), количество
аргументов и их типы (а иногда и имена аргументов), тип результата.
- [Метод / Method](https://github.com/HowProgrammingWorks/Function)
  - функция или процедура, связанная с объектным контекстом или программным интерфейсом;
  - `{ a: 10, b: 10, sum() { return this.a + this.b; } }`
- [Цикл / Loop](https://github.com/HowProgrammingWorks/Iteration)
  - многократное исполнение блока операторов
- [Условие / Conditional statements](https://github.com/HowProgrammingWorks/Conditional)
  - синтаксическая конструкция, позволяющая выполнить разные действия или
  возвращающая разные значения (тернарный оператор) в зависимости от логического
  выражения (возвращающего true или false)
- [Рекурсия / Recursion](https://github.com/HowProgrammingWorks/Recursion) -
задание алгоритма вычисления функции через вызов ее самой (прямой или непрямой)
или определение функции, через нее саму.
  - Косвенная (непрямая) рекурсия - когда функция определена или вызывает себя
  не напрямую, а через другую или цепочку функций;
  - Хвостовая - частный случай, когда рекурсивный вызов является последней
  операцией перед возвратом значения, что всегда может быть преобразовано
  в цикл, даже автоматическим способом. Не хвостовая тоже может быть
  преобразована в цикл и оптимизирована, но более сложным способом, обычно
  вручную.
- [Строка / String](https://github.com/HowProgrammingWorks/String)
  - последовательность символов (в большинстве языков к каждому символу можно
  обратиться через синтаксис доступа к элементам массива, например, квадратные
  скобки).
- [Коллекция / Collection](https://github.com/HowProgrammingWorks/Collections) -
структура данных, служащая для хранения набора значений и предоставляющая доступ
к ним по индексам или ключам.
- Массив / Array - коллекция элементов, доступ к которым осуществляется по
индексам. Пример: `const cities = ['Tehran', 'Yalta', 'Potsdam'];`
- Отладка / Debug - процесс обнаружения и устранения ошибок в программном
обеспечении при помощи вывода сообщений или инструментов: отладчика,
профилировщика, декомпилятора, систем мониторинга ресурсов и логирования,
систем непрерывной интеграции и тестирования.
- ЦП / CPU - центральный процессор / central processing unit - устройство,
выполняющее машинные инструкции.
- АЛУ / ALU - блок ЦП, выполняющий арифметические и логические преобразования
над машинными словами, представляющими целые числа, числа с плавающей точкой,
адресами памяти, строками, логическими величинами.
- Компонент / Component - несколько программных объектов (например: функций,
классов, монад, типов) объединенных и организованных по общему признаку.
- Модуль / Module - целостный, функционально полный, независимый компонент
программной системы имеющий имя, интерфейс, реализацию.
- [Модульность / Modularity](https://github.com/HowProgrammingWorks/Modularity)
  - модульность повышает переиспользование кода, упрощает интеграцию компонентов,
  улучшает компоновку и тестирование программ по частям;
  - ограничения: модули не должны использовать глобальные переменные или
  модифицировать базовые классы/прототипы/функции языка программирования,
  платформы и/или фреймворка; модули должны быть слабо связаны, а
  взаимодействовать друг с другом должны через внешнее API (предпочтительно)
  или шину событий (если система построена на событийной модели, подписке).
- Библиотека / Library - сборник программных объектов (например: функций,
классов, монад, типов) подготовленный для повторного использования (часто
опубликованный). Библиотека это более крупная логическая часть кода, чем
компонент. Иногда библиотеку используют как синоним модуля, а иногда библиотека
состоит из нескольких модулей.
- Сложность / Complexity
  - Вычислительная сложность / Computational complexity
  - Колмогоровская (описательная) сложность / Kolmogorov (descriptive) complexity
  - Если нет циклов, то описательная коррелирует с вычислительной

## Asosiy tushunchalar

- [Объект или Экземпляр / Object or Instance](https://github.com/HowProgrammingWorks/DataTypes) -
структура данных, содержащая состояние и методы, связанные с этим состоянием.
Объект может быть создан как литерал `{}` или экземпляр класса `new ClassName()`
или как экземпляр прототипа `new PrototypeConstructor()` или возвращен из фабрики.
  - `const person = { name: 'Marcus', city: 'Roma', born: 121 };`
  - `const person = new Person('Marcus', 'Roma', 121);`
- [Класс / Class](https://github.com/HowProgrammingWorks/Prototype) -
программная абстракция, объединяющая состояние и поведение (свойства и методы)
своих экземпляров (инстансов).
  - `class Point { constructor(x, y) { this.x = x; this.y = y; } }`
  - `class Rect { move(x, y) { this.x += x; this.y += y; } }`
  - `class Square extends Rect { constructor(x, y, m) { super(x, y, m, m); } }`
  - `class Point { static from(point) { return new Point(this.x, this.y); } }`
- [Прототип / Prototype](https://github.com/HowProgrammingWorks/Prototype) -
специальный объект, на который ссылаются его экземпляры и наследники. Свойства
прототипа становятся видны у наследников, если эти свойства не переопределены у
наследников. Формируется цепочка прототипов, по которой происходит
последовательный поиск свойств, пока они не будут найдены или пока не будет
достигнут конец цепочки наследования. Иногда под прототипом понимается шаблон,
который клонируется во время инстанциирования (не для JavaScript).
- Инстанцирование / Instantiation - создание объекта (экземпляра) или выделение
памяти для структуры данных.
  - `const rect = new Rectangle(-50, -50, 100, 150);`
  - `const rect = { a: { x: -50, y: -50 }, b: { x: 100, y: 150 } };`
  - `const cities = new Array(1000);`
  - `const cities = ['Tehran', 'Kiev', 'Yalta', 'Beijing', 'Potsdam', 'London'];`
- Область видимости / Scope - часть кода, из которой "виден" идентификатор.
- Лексический контекст / Lexical environment - набор идентификаторов, связанных
с определенными значениями в рамках функции или блока кода (в том числе блоков
циклов, условий и т.д.).
- Объектный контекст функции - объект, связанный со служебным идентификатором
`this`. Все функции, кроме стрелочных, могут быть связаны с объектным контекстом.
Объект связан с `this` если функция является методом этого объекта, если функция
привязана к нему через `bind` или вызвана через `apply` и `call`.
- Глобальный контекст / Global context - глобальный объект-справочник. Если
идентификатор не находится ни в одном из вложенных лексических контекстов, то
будет выполнен его поиск в глобальном контексте (global, window, sandbox).
- Объявление функции / Function definition - способ объявления функции, который
виден из любого места в лексическом контексте, в котором объявлена функция,
пример: `function sum(a, b) { return a + b; }`
- Функциональное выражение / Function expression - связывание функции с
идентификатором при помощи присвоения, при котором значение будет доступно через
идентификатор не во всем лексическом контексте, а только после места присвоения.
Имеет несколько синтаксических вариантов:
  - функциональное выражение с именованной функцией / Named function expression
    - `const max = function max(a, b) { return a + b; };`
  - анонимное функциональное выражение / Anonymous function expression
    - `const max = function(a, b) { return a + b; };`
  - лямбда-функция / Lambda function
    - `const max = (a, b) => { return a + b; };`
  - лямбда-выражение, Функция-стрелка / Lambda expression, Arrow function
    - `const max = (a, b) => (a + b);`
- [Чистая функция / Pure Function](https://github.com/HowProgrammingWorks/Function)
  - функция, вычисляющая результат только на основе аргументов, не имеющая
  состояния и не обращающаяся к операциям ввода-вывода
  - функция, результат которой всегда детерминированный, т.е. для любого
  аргумента всегда будет один и тот же результат
  - функция, не имеющая побочных эффектов (см. побочный эффект)
- [Замыкание / Closure](https://github.com/HowProgrammingWorks/Closure)
  - если вернуть функцию `g` из функции `f`, то `g` будет видеть контекст
  функции `f`, так же, как и свои аргументы;
  - если `f` возвращает `g`, то говорят, что экземпляр `g` замкнул контекст `f`;
  - способ, позволяющий связать функцию с контекстом (с данными или
  переменными контекста);
  - замыкание является аналогом свойств в ООП, тоже связывающие свойства с
  методами через объект, по сути объект в ООП сам является контекстом
  связывания;
  - при помощи замыкания можно реализовать функциональное наследование;
  - `const add = a => b => a + b;`
  - `const hash = (data = {}) => (key, value) => (data[key] = value, data);`
- [Суперпозиция / Superposition](https://github.com/HowProgrammingWorks/Composition)
  - объединение вызова функций в выражения таким образом, что результат одних
  функций становится аргументами других функций;
  - `const expr2 = add(pow(mul(5, 8), 2), div(inc(sqrt(20)), log(2, 7)));`
- [Композиция / Composition](https://github.com/HowProgrammingWorks/CompositionИнструкция / Instruction - один шаг алгоритма вычислений, например инструкция процессора исполняется CPU.
Оператор / Statement - наименьшая синтаксическая часть языка программирования, исполняемая интерпретатором, средой или компилируемая в машинный код.
Команда / Command - атомарная задача для командного процессора.
Выражение / Expression - синтаксическая конструкция языка программирования предназначенная для выполнения вычислений. Выражение состоит из идентификаторов, значений, операторов и вызова функций. Пример: (len - 1) * f(x, INTERVAL)
Блок кода / Block - логически связанная группа инструкций или операторов. Блоки создают область видимости. Блоки могут быть вложенными. Примеры: {}, (+ a b), begin end, отступы в Python.
Процедура или подпрограмма / Procedure or Subroutine - логически связанная группа инструкций или операторов, имеющая имя. Процедура способствует повторному использованию кода и может быть вызвана из разных частей программы, много раз и с разными аргументами. Процедура не возвращает значений, в отличие от функций, но в некоторых языках (но не в JavaScript) может модифицировать свои аргументы. Во многих языках процедура описывается при помощи синтаксиса функций (например, типа void).
Функция / Function - абстракция преобразования значений. Функция однозначно отображает одно множество значений в другое множество значений. Функция может быть задана блоком операторов или выражением. Функция имеет набор аргументов. Функция может быть вызвана по имени или через указатель. Функция способствует повторному использованию кода и может быть вызвана из разных частей программы, много раз и с разными аргументами. В JavaScript функция описывается при помощи function или синтаксиса стрелок (лямбда-функций).
Сигнатура функции / Function signature - имя (идентификатор), количество аргументов и их типы (а иногда и имена аргументов), тип результата.
Метод / Method
функция или процедура, связанная с объектным контекстом или программным интерфейсом;
{ a: 10, b: 10, sum() { return this.a + this.b; } }
Цикл / Loop
многократное исполнение блока операторов
Условие / Conditional statements
синтаксическая конструкция, позволяющая выполнить разные действия или возвращающая разные значения (тернарный оператор) в зависимости от логического выражения (возвращающего true или false)
Рекурсия / Recursion - задание алгоритма вычисления функции через вызов ее самой (прямой или непрямой) или определение функции, через нее саму.
Косвенная (непрямая) рекурсия - когда функция определена или вызывает себя не напрямую, а через другую или цепочку функций;
Хвостовая - частный случай, когда рекурсивный вызов является последней операцией перед возвратом значения, что всегда может быть преобразовано в цикл, даже автоматическим способом. Не хвостовая тоже может быть преобразована в цикл и оптимизирована, но более сложным способом, обычно вручную.
Строка / String
последовательность символов (в большинстве языков к каждому символу можно обратиться через синтаксис доступа к элементам массива, например, квадратные скобки).
Коллекция / Collection - структура данных, служащая для хранения набора значений и предоставляющая доступ к ним по индексам или ключам.
Массив / Array - коллекция элементов, доступ к которым осуществляется по индексам. Пример: const cities = ['Tehran', 'Yalta', 'Potsdam'];
Отладка / Debug - процесс обнаружения и устранения ошибок в программном обеспечении при помощи вывода сообщений или инструментов: отладчика, профилировщика, декомпилятора, систем мониторинга ресурсов и логирования, систем непрерывной интеграции и тестирования.
ЦП / CPU - центральный процессор / central processing unit - устройство, выполняющее машинные инструкции.
АЛУ / ALU - блок ЦП, выполняющий арифметические и логические преобразования над машинными словами, представляющими целые числа, числа с плавающей точкой, адресами памяти, строками, логическими величинами.
Компонент / Component - несколько программных объектов (например: функций, классов, монад, типов) объединенных и организованных по общему признаку.
Модуль / Module - целостный, функционально полный, независимый компонент программной системы имеющий имя, интерфейс, реализацию.)
  - `const compose = (f1, f2) => x => f2(f1(x));`
  - `const compose = (...funcs) => (...args) => (funcs.reduce((args, fn) => [fn(...args)], args));`
- [Частичное применение / Partial application](https://github.com/HowProgrammingWorks/PartialApplication)
  - `const partial = (fn, x) => (...args) => fn(x, ...args);`
- [Каррирование / Currying](https://github.com/HowProgrammingWorks/PartialApplication)
  - `const result = curry((a, b, c) => (a + b + c))(1, 2)(3);`
- [Побочные эффекты / Side effects](https://github.com/HowProgrammingWorks/Function)
- [Функция высшего порядка / Higher-order Function](https://github.com/HowProgrammingWorks/HigherOrderFunction)
  - если функция только в аргументах, то это колбек;
  - если функция только в результате, то это фабрика функций на замыканиях;
  - если возвращаемая функция имеет тот же смысл, что и получаемая в
  аргументах (+ дополнительное поведение), то это обертка;
  - очень редко бывает, что возвращаемая функция не связана с функцией из
  аргументов (но пока ни кто не нашел вразумительного примера, где это
  реально нужно);
  - если на выходе класс или функция-конструктор, то это фабрики классов и
  прототипов соответственно;
- Функциональное наследование / Functional Inheritance - при помощи замыканий,
частичного применения, каррирования, вложенных лямбд.
- [Обертка / Wrapper](https://github.com/HowProgrammingWorks/Wrapper)
  - функция, которая оборачивает другую функцию (иногда объект, интерфейс или
  функциональный объект), добавляя ему дополнительное поведение;
  - можно обернуть целый API интерфейс и даже асинхронную функцию вместе с
  колбеками (если известен контракт);
- [Дженерики / Generics](https://github.com/HowProgrammingWorks/Generics)
  - Обобщенное программирование - парадигма, позволяющая обобщенно описать
  алгоритмы и структуры данных, абстрагируясь от конкретных типов.
- Интерфейс / Interface
  - набор методов (функций) объединенных или общим объектным контекстом или
  применением к структурам данных одной предметной области т.е. смыслом (API);
  - способ определения (спецификации) контракта, по которому связаны
  программные компоненты;
  - Набор методов с их именами, аргументами и типами аргументов
- Программный интерфейс / Application Interface, API
  - интерфейс программных компонентов: модулей, слоев абстракции, приложений;
- [Синглтон / Singleton](https://github.com/HowProgrammingWorks/Singleton)
  - шаблон проектирования, предполагающий, что в одном пространстве имен
  (процессе, приложении, базе данных) будет только один экземпляр класса
  (или просто один подобный объект) к которому можно обратиться по определенному
  (известному) имени;
- [Функция обратного вызова, колбек / Callback](https://github.com/HowProgrammingWorks/Callbacks)
  - функция передаваемая в качестве аргумента в другую функцию (или метод)
  для того, чтобы быть вызванной для возврата значения, ошибки или уведомления;
  - функции обратного вызова имеют подтипы:
    - один раз вызываемые (чаще всего);
    - [Событие / Event](https://github.com/HowProgrammingWorks/Callbacks)
    - [Лисенер / Listener](https://github.com/HowProgrammingWorks/Callbacks)
- [Итерирование / Iteration](https://github.com/HowProgrammingWorks/Iteration) -
многократное повторение одного блока кода или одной функции над различными
данными: элементами массивов, множеств, списков, коллекций и различными
значениями переменной цикла.
- [Итератор / Iterator](https://github.com/HowProgrammingWorks/Iteration) -
интерфейс доступа к элементам коллекции: массива, множества, списка;
- [Файл / File](https://github.com/HowProgrammingWorks/Files)
- [Поток, Файловый поток / Stream, File Stream](https://github.com/HowProgrammingWorks/Streams)
- [Сокет / Socket](https://github.com/HowProgrammingWorks/Socket) -
программный интерфейс (или абстракция) для обмена данными между процессами.
- [Дескриптор / Handle](https://github.com/HowProgrammingWorks/Files) -
уникальный идентификатор программного объекта (чаще всего объекта операционной
системы): файла, сокета, окна, таймера, соединения и т.д.
- Состояние / State - совокупность данных программного компонента (переменных
и структур данных), определяющие его поведение и реакцию на операции с ним.
- Кэш / Cache - место временного хранения данных (буфер, коллекция, область
памяти) для быстрого доступа и оптимизации. Возможно кэширование операций
чтения, вычислений, операций записи (когда запись не может быть произведена
достаточно быстро) или упреждающее чтение в буфер (когда можно определить,
какие данные будут запрошены с наибольшей вероятностью).
- Хэширование / Hashing - преобразование данных произвольной длины (буфера,
массива, объекта или структуры данных) в последовательность битов определенной
длины (хеш) при помощи хеш-функции (при изменении хоть 1 бита в данных хеш
меняется существенно).
- [Функциональный объект](https://github.com/HowProgrammingWorks/Functor) -
объект функционального типа, который является функцией и объектом одновременно.
Другими словами, функциональный объект может быть вызван, как функция и может
иметь свойства и методы, как объект.
- [Функтор / Functor](https://github.com/HowProgrammingWorks/Functor) - это
функциональный объект, который является еще и рекурсивным замыканием. Функтор
хранит в замыкании защищенное значение и позволяющий отобразить это значение
в другой функтор через вызов функции (обычно `map`).
- [Аппликативный функтор](https://github.com/HowProgrammingWorks/Functor) -
функтор, который имеет метод `apply`.
- Монада / Monad - аппликативный функтор, который имеет метод `chain`.
- [Мемоизация / Memoization](https://github.com/HowProgrammingWorks/Memoization) -
обертка, сохраняющая результаты выполнения функции для предотвращения повторных
вычислений.
- [Примесь / Mixin](https://github.com/HowProgrammingWorks/Mixin) - добавление
свойств, методов или поведения к объекту после его инстанциирования. Пример:
`Object.assign(target, { field1, field2 }, { field3 });`
- Декоратор / Decorator - шаблон оборачивания объектов или функций для добавления
новой функциональности без наследования при помощи специального синтаксиса.
- [Наследование / Inheritance](https://github.com/HowProgrammingWorks/Inheritance)
- [Множественное наследование / Multiple Inheritance](https://github.com/HowProgrammingWorks/Inheritance)
- [Непрямое наследование / Indirect Inheritance](https://github.com/HowProgrammingWorks/Inheritance)
- [Генератор / Generator](https://github.com/HowProgrammingWorks/Generator)
- [Итератор / Iterable and Iterator](https://github.com/HowProgrammingWorks/Iterator)
- [Ввод/вывод / I/O, Input-output](https://github.com/HowProgrammingWorks/AsynchronousProgramming)
  - операции, выходящие за рамки CPU и RAM (арифметико-логического устройства
  и памяти), т.е. операции с устройствами ввода вывода: сеть, диск, порты,
  консоль (клавиатура и экран), другие периферийные устройства (взаимодействие
  с которыми на порядки медленнее, чем внутренние операции в АЛУ и памяти);
- [EventEmitter](https://github.com/HowProgrammingWorks/EventEmitter)
  - универсальная абстракция для работы с событиями через подписку (subscription:
  addListener, on, once) и отправку (emit)
- [Чеининг / Chaining](https://github.com/HowProgrammingWorks/Chaining)
  - цепочный синтаксис вызова функций `total(april)(may)(july)` или методов
  `array.filter(f1).reduce(f2)`
- [Сериализация / Serialization](https://github.com/HowProgrammingWorks/Serialization) -
преобразование структуры данных (развернутой в памяти) в битовую
последовательность, обычно в последовательность байтов (бинарная сериализация)
или в строку (текстовая сериализация).
- [Десериализация / Deserialization](https://github.com/HowProgrammingWorks/Serialization) -
операция, обратная сериализации, т.е. восстановление структуры данных из
последовательности битов (чаще байтов или строки).
- Парсинг / Parsing - синтаксический анализ текста, результатом чего может являться:
  - для формальной грамматики - AST-дерево;
  - для слабоструктурированного документа - структура данных, имеющая
  четкую структуру, в которую частично перенесены данные из слабой структуры;
  - для других естественных или искусственных языков - информационные модели,
  им соответствующие;
- [Регулярные выражения / Regular Expressions](https://github.com/HowProgrammingWorks/RegExp) -
синтаксическая конструкция, паттерн, формальный язык, определяющий порядок
парсинга другой синтаксической конструкции.
- [Зависимость / Dependency](https://github.com/HowProgrammingWorks/Project) -
связанность программных компонентов, при которой один компонент (зависимый)
"знает" другой; это значит, что в нем помещен вызов метода (реализация которого
содержится в другом) или он слушает событие, которое генерирует другой или он
"знает" структуры данных, которые могут быть переданы из другого компонента.
- Декомпозиция / Decomposition - разделение программного компонента на части по
принципу функциональности, при этом, каждая часть будет решать подзадачу и
появится часть кода, которая определяет порядок связи всех частей (композицию).
- [Ленивость / Lazy](https://github.com/HowProgrammingWorks/Lazy)
- [Обработка ошибок / Error handling](https://github.com/HowProgrammingWorks/Errors)
- [Фабрика / Factory](https://github.com/HowProgrammingWorks/Factory) - функция
или метод для инстациирования объектов, функций, структур данных и любых других
программных абстракций, например, экземпляров класса в обход конструктора или
функциональных объектов.
- Объектный Пул / [Object Pool](https://github.com/HowProgrammingWorks/Pool) -
Множество заранее инстанциированных объектов (или массивов, сокетов, буферов,
структур данных и других программных абстракций) из которого мы можем их брать
инициализированные экземпляры (вместо инстанциирования новых) и отдавать их
после использования.
- [Таймеры / Timers](https://github.com/HowProgrammingWorks/Timers)
- [Адаптер / Adapter](https://github.com/HowProgrammingWorks/Adapter) -
Паттерн достижения совместимости, позволяющий обернуть класс, функцию или
другой программный компонент с несовместимым контрактом в программный
компонент с контрактом, который нам нужен.
- [Стратегия (Strategy)](https://github.com/HowProgrammingWorks/Strategy) -
Паттерн реализует выбор одного из совместимых и взаимозаменяемых классов,
которые содержат поведение (алгоритм), аналогичный по функциональности и
реализующий общий интерфейс. Актуален и для функционального программирования.
- [Фасад / Facade](https://github.com/HowProgrammingWorks/Facade) - Паттерн
для скрытия сложности. Фасад скрывает несколько инстансов разных классов в
своих свойствах (иногда приватных, но для JS этого пока нет) и предоставляет
общий (фасадный) интерфейс для управления ими. Для функционального
программирования возможен аналог фасада - функция обертка, скрывающая
инстансы в своем контексте и предоставляющая доступ к ним через возврат
функции (с замыканием) или другого инстанса (методы которого тоже имеют
доступ к скрываемым инстансам через замыкание).

## Yordamchi materiallar

- [Линтер / Linter](https://github.com/HowProgrammingWorks/Tools) - статический
анализатор кода (без запуска), который может определить и предложить
стилистические, грамматические или оптимизационное улучшение или просто выявить
проблему (а иногда и исправить ее автоматически).
- Система контроля версий
- Менеджер пакетов
- Непрерывная интеграция
- Тестирование

## Ma'lumotlar tuzulmasi

- [Запись или структура / Struct or Record](https://github.com/HowProgrammingWorks/DataStructures)
- [Массив / Array](https://github.com/HowProgrammingWorks/DataStructures)
- [Буфер / Buffer](https://github.com/HowProgrammingWorks/Buffers)
- [Список / List](https://github.com/HowProgrammingWorks/LinkedList)
  - Односвязный, двусвязный, кольцевой, развернутый список (список массивов)
  - Реализация на объектах, массивах и замыканиях
  - Реализация на синтаксисе прототипов, классов и фабрик
  - Реализация на замыканиях и функциональных объектах
  - Реализация на одной и двух категориях (только узел или список и узел)
- [Стек, очередь, дек](https://github.com/HowProgrammingWorks/Dequeue)
  - Стек / Stack - список, работающий по принципу LIFO;
  - Очередь / Queue - список, работающий по принципу FIFO;
  - Дек / Dequeue - двухсторонний список, работающий, как стек и очередь;
- [Дерево](https://github.com/HowProgrammingWorks/Trees)
- [Двоичное дерево](https://github.com/HowProgrammingWorks/Trees), поисковое
дерево, красно-черное дерево.
- Куча / Heap - древовидная структура данных или область памяти для динамического
распределения под хранение данных.
- [Граф / Graph](https://github.com/HowProgrammingWorks/Graph)
- [Буфер / Buffer](https://github.com/HowProgrammingWorks/Buffers) -
область памяти для хранения данных (обычно для операций ввода/вывода).
- Типизированные массивы
- [Коллекция / Collection](https://github.com/HowProgrammingWorks/Collections) -
структура данных, служащая для хранения набора значений и предоставляющая
доступ к ним по индексам или ключам.
- [Множество / Set](https://github.com/HowProgrammingWorks/Set)
  - структура данных, реализующая математическое "множество";
  - структура данных, служащая для хранения однородного набора значений, которые
  не имеют индексов или ключей (но внутри структуры данных они должны иметь
  порядок, например, индекс в массиве, однако, множество абстрагирует нас от
  этой особенности реализации).
- [Ключ-значение, Хешмап / Map, Key-value](https://github.com/HowProgrammingWorks/KeyValue)
  - [класс `Map`](https://github.com/HowProgrammingWorks/Map)

## Kengaytirilgan tushunchalar

- [Сборка мусора / Garbage Collection](https://github.com/HowProgrammingWorks/GarbageCollection)
- [Прокси / Proxy](https://github.com/HowProgrammingWorks/Proxy)
- [Символ / Symbol](https://github.com/HowProgrammingWorks/Symbol)
- [Дифер / Deferred](https://github.com/HowProgrammingWorks/Callbacks)
- [Промис / Promise](https://github.com/HowProgrammingWorks/Promise)
- [Необработанные ошибки в промисах на Node.js](https://github.com/HowProgrammingWorks/PromiseError)
- [Фьючер / Future](https://github.com/HowProgrammingWorks/Callbacks)
- [Коллекторы данных / Data and Key Collectors](https://github.com/metarhia/metasync/blob/master/lib/collector.js)
- Неизменяемые данные / Immutable Data
- Изменяемые данные / Mutable Data
- Интроспекция / Introspection
- Рефлексия / Reflection
- Скаффолдинг / Scaffolding
- [Инверсия управления / IoC, Inversion of Control](https://github.com/HowProgrammingWorks/InversionOfControl)
- [Внедрение зависимостей / DI, Dependency Injection](https://github.com/HowProgrammingWorks/DependencyInjection)
- [Межпроцессовое взаимодействие / IPC, Interprocess Communication](https://github.com/HowProgrammingWorks/InterProcessCommunication)
- [Песочница / Sandbox](https://github.com/HowProgrammingWorks/Sandboxes)
- Архитектура / Architecture
- Слой доступа к данным / Data Access Layer
- Курсор / Cursor
- Объектно-реляционное отображение / ORM, Object-relational Mapping
- [Сервер / Server](https://github.com/HowProgrammingWorks/NodeServer)
  - [Приклеивание по IP или идентификатору сессии / IP or Session Sticky](https://github.com/HowProgrammingWorks/NodeServer/tree/master/ip-sticky)
  - Кластеризация / Cluster mode
    - При помощи [cluster](https://github.com/HowProgrammingWorks/NodeServer/tree/master/native-cluster)
    - при помощи [child_process](https://github.com/HowProgrammingWorks/NodeServer/tree/master/native-cp)
  - [Разработка API (клиент и сервер)](https://github.com/HowProgrammingWorks/API)
- Сервер приложений / Application Server
- Тонкий клиент и толстый клиент
- [Проекция данных / Projection](https://github.com/HowProgrammingWorks/Projection)
- [Измерение производительности / Benchmarking](https://github.com/HowProgrammingWorks/Benchmark)
- [Интерфейс командной строки / CLI, Command Line Interface and Console](https://github.com/HowProgrammingWorks/CommandLine)
- [Мониторинг файловой системы / File System Watching](https://github.com/HowProgrammingWorks/FilesystemWatch)
- [Транзакционные объекты/Transaction](https://github.com/HowProgrammingWorks/Transaction)
- [Метаданные / Metadata](https://github.com/HowProgrammingWorks/Metaprogramming)
- [Протокол / Protocol](https://github.com/metarhia/metacom)
- [Динамическая загрузка модулей / Live Code Reload](https://github.com/HowProgrammingWorks/LiveReload)
- Http Request (HTTP, XMLHttpRequest, fetch): [примеры](https://github.com/HowProgrammingWorks/HttpRequest)
- [Неблокирующие итерации](https://github.com/HowProgrammingWorks/NonBlocking)
- [Линзы - функциональные аналоги геттера и сеттера](https://github.com/HowProgrammingWorks/Lenses)

## Asinxron dasturlash

- Асинхронное программирование / Asynchronous Programming
- Неблокирующая операция / Non-blocking I/O
- Асинхронное итерирование / Asynchronous Iterable
- Асинхронный коллектор данных / Asynchronous data collector
- Промис / Promise
- Генератор / Generator Function
- Асинхронный генератор / Asynchronous Generator Function
- Итератор / Iterator
- Асинхронный итератор / Asynchronous Iterator
- Итерируемый объект / Iterable
- Асинхронная композиция функций / Asynchronous Function Composition
- Thenable
- async/await
- Асинхронная очередь / Asynchronous Queue
- Открытый конструктор / Revealing Constructor
- Фьючер / Future
- Дифер / Deferred
- Модель акторов / Actor Model
- Наблюдатель / Observer
- Поток событий / Event stream

## Parallel dasturlash

- Состояние гонки / Race Condition - состояние в многопоточной или конкурентной
программной системе, когда несколько потоков исполнения конкурируя за общий
ресурс портят данные, приводят к непредусмотренному порядку исполнения,
зацикливаются, и т.д., что приводит к утечке ресурсов, непредсказуемому и
неправильному поведению, уязвимостям, нестабильности работы.
- Взаимная блокировка / Deadlock - состояние в многопроцессовой (распределенной)
системе, когда несколько процессов захватили ресурсы, необходимые для дальнейшей
работы друг друга, заблокировав, тем самым дальнейшую работу.
- Livelock - зацикленная блокировка, бесконечно изменяющая состояние, но не
выполняющая полезной работы.
- Ресурсный голод / Resource starvation - состояние в программной системе (обычно
многопоточной), когда она постоянно запрашивает доступ к ресурсам (обычно
разделяемым), и не может их получить.
- Критическая секция / Critical section - участок исполняемого кода, в котором
производится эксклюзивный доступ к разделяемому ресурсу.
- [Потоки / Threads](https://github.com/HowProgrammingWorks/Threads)
  - SharedArrayBuffer
  - worker_threads в Node.js
- [Атомарные операции / Atomics](https://github.com/HowProgrammingWorks/Atomics)
- [Семафор / Semaphore](https://github.com/HowProgrammingWorks/Semaphore)
- [Мьютекс / Mutex](https://github.com/HowProgrammingWorks/Mutex)

## Dasturlash paradigmalari

- [Императивное программирование / Imperative Programming](https://github.com/HowProgrammingWorks/ImperativeProgramming)
  - Неструктурное программирование / Non-structured
  - Структурное программирование / Structured Programming
  - Процедурное программирование / Procedural Programming
  - [Object-oriented programming](https://github.com/HowProgrammingWorks/ObjectOrientedProgramming)
  - [Prototype-oriented programming](https://github.com/HowProgrammingWorks/PrototypeOrientedProgramming)
- [Функциональное программирование / Functional Programming](https://github.com/HowProgrammingWorks/FunctionalProgramming)
  - [примеры разных стилей функционального кода](https://github.com/HowProgrammingWorks/Abstractions)
- Логическое программирование / Logical Programming
- Декларативное программирование / Declarative Programming
- [Программирование управляемое данными / Data-driven Programming](https://github.com/HowProgrammingWorks/DataDrivenProgramming)
- Техники программирования
  - [Асинхронное программирование / Asynchronous Programming](https://github.com/HowProgrammingWorks/AsynchronousProgramming)
  - Реактивное программирование / Reactive Programming
- [Событийное программирование / Event-driven Programming](https://github.com/HowProgrammingWorks/EventDrivenProgramming)
- [Метапрограммирование / Metaprogramming](https://github.com/HowProgrammingWorks/Metaprogramming)
