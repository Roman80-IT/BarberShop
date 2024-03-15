# BarberShop

---

💈 🪒
[Посилання на макет](https://www.figma.com/file/z6Rb84e4NKxe66QNokOWA8/Barbershop-EN?node-id=1374%3A32)

---

## Markdown:

1. Заголовки - використовуються символи "#" для позначення заголовків різних рівнів:

```
# Заголовок 1 рівня
## Заголовок 2 рівня
### Заголовок 3 рівня
```

2. Виділення тексту:
   `Курсив` - використовуються одинарні символи підкреслення або зірочки _текст_ або _текст_
   `Напівжирний` - подвійні символи підкреслення або зірочки **текст** або **текст**

3. Списки:

- `Нумеровані списки`: використовуються числа з крапкою

```
1. Перший пункт
2. Другий пункт
```

- `Ненумеровані списки`: використовуються символи `дефісу -`, `плюса +` або `зірочки \*`

```
- Перший пункт

* Другий пункт

- Третій пункт
```

4. Посилання: [Текст посилання](https://приклад.com)
5. Зображення: ![Альтернативний текст](https://приклад.com/зображення.jpg)
6. Коди та цитати:
   Коди вставляються в рядок за допомогою одинарних апострофів `код`
   Багаторядкові коди обрамлюються потрійними апострофами:

```
// коментар
код
код
```

Цитати позначаються символом `>`

`> Це цитата`

7. Нові рядки: Для створення нового рядка в Markdown необхідно залишити порожній рядок між абзацами. Або використати два пробіли в кінці рядка і натиснути `Enter`.

---

## Step 1.1:

**HTML (HyperText Markup Language)** - це мова розмітки документів, яка використовується для створення структури та контенту веб-сторінок.

- **Теги та атрибути**:
  `Теги` - це елементи, які визначають структуру та семантику вмісту сторінки.
  `Атрибути` - це додаткові властивості, які можна додати до тегів для надання більшої інформації або функціональності.

- **Cкелет HTML-документа**:
  `<!DOCTYPE html> `- оголошення типу документа.
  `<html>...</html>` - корінний елемент документа.
  `<head>...</head>` - містить метадані про документ.
  `<body>...</body>` - містить весь відображуваний контент сторінки.

- **Метаінформація документа**:
  <title>...</title> - задає заголовок документа, який відображається на вкладці браузера.
  <meta> - використовується для визначення метаданих документа, таких як кодування, опис, ключові слова тощо.
  Поняття семантичної розмітки: Семантична розмітка - це використання відповідних тегів для представлення їх змісту та значення, а не лише для візуального форматування.

- **Семантична розмітка**

* **Розмітка тексту**:
  `<p>...</p>` - для абзаців тексту.
  `<h1>...</h1>, <h2>...</h2> ... <h6>...</h6>` - для заголовків різних рівнів.
  `<ol>...</ol>` та `<ul>...</ul> `- для впорядкованих та невпорядкованих списків.
  `<a>...</a>` - для створення гіперпосилань.

* **Зображення**:
  `<img src="..." alt="...">` - для вставки зображень на сторінку.

  `<figure>...</figure>` - для групування зображень та підписів до них.

- **Секційні теги**:
  `<header>...</header>` - для представлення заголовка сторінки або розділу.  
  `<footer>...</footer>` - для представлення нижнього колонтитулу сторінки або розділу.  
  `<main>...</main>` - для визначення основного контенту сторінки.  
  `<section>...</section>` - для групування контенту за темами або розділами.  
  `<nav>...</nav>` - для представлення навігаційних посилань.  
  `<article>...</article>` - для визначення незалежного контенту, наприклад, статті або запису в блозі.  
  `<aside>...</aside>` - для визначення другорядного контенту, наприклад, бічної панелі.

- **Інтерактивні елементи**
  дозволяють користувачеві взаємодіяти з веб-сторінкою. Ось деякі з найпоширеніших інтерактивних елементів:

_Форми_ (`<form>`): Форми використовуються для збирання даних від користувача, таких як текстові поля, випадаючі списки, прапорці та кнопки. Усередині форми можна використовувати такі елементи:

`<input>` (текстові поля, прапорці, радіокнопки, кнопки тощо)  
`<textarea>` (многорядкове текстове поле)  
`<select>` (випадаючий список)  
`<button>` (кнопка)

_Посилання_ (`<a>`): Посилання дозволяють користувачеві переходити на інші веб-сторінки або виконувати певні дії (наприклад, завантажувати файл або відправляти електронний лист).

_Елементи мультимедіа_:
`<video>` (для вбудовування відеоплеєра)
`<audio>` (для вбудовування аудіоплеєра)

_Елементи Canvas_ (`<canvas>`) та SVG (`<svg>`): Використовуються для створення інтерактивної графіки та анімацій на веб-сторінці.

_Діалогові вікна_ (`<dialog>`): Елемент для створення модальних або немодальних діалогових вікон.

_Типи кнопок_:

---

`<button>`: Елемент `<button>` є основною кнопкою у **HTML**. Він може містити текст, зображення або інші вкладені елементи, і використовується для запуску JavaScript-подій або виклику дій:

```html
<button>Натисніть мене</button>
```

`<input type="button">`: Елемент `<input>` може бути використаний для створення кнопки зазначеного типу. Тип **button** вказує, що це кнопка:

```html
<input type="button" value="Натисніть мене" />
```

для елемента <button> в HTML:

type="button": Цей тип кнопки призначений для створення звичайної кнопки, яка не відправляє форму та не викликає жодних стандартних дій:

```html
<button type="button">Натисніть мене</button>
```

---

`type="submit"`: Цей тип кнопки використовується для відправки форми на сервер. При натисканні на кнопку відправляється запит на сервер з введеними даними форми:

```html
<input type="submit" value="Відправити" />
```

html
<button type="submit">Відправити</button>

---

`<input type="reset">`: Цей тип кнопки використовується для скидання значень форми до їхніх початкових значень:

```html
<input type="reset" value="Скинути" />
```

```html
<button type="reset">Скинути</button>
```

---

`type="image"`: Цей тип кнопки використовується для створення кнопки зображення. Коли користувач клацне на зображення, координати клацання відправляються разом із відправленою формою:

```html
<input type="image" src="button_image.png" alt="Натисніть мене" />
```

```html
<button type="image" src="button_image.png" alt="Натисніть мене"></button>

Це лише деякі з типів кнопок, які можна використовувати в HTML. Ці атрибути
дозволяють керувати поведінкою кнопок
<button>в HTML та надають більшу гнучкість у їхньому використанні. ---</button>
```

! В `посилання` не можна вкладати `кнопки` та в `кнопки` не бажано вкдладати `посилання`

! Альтернативне використання `<a>` - без `href` в меню для вимкнення пунктів меню

````

- **Абсолютний та відносний шлях до файлу**:
  `Абсолютний шлях` - це повний шлях до файлу, починаючи з кореня веб-сервера або дисковим шляхом.
  `Відносний шлях` - це шлях до файлу відносно поточного розташування HTML-документа.
- **Валідація HTML-документа**: Валідація - це процес перевірки коректності HTML-коду відповідно до стандартів та специфікацій. Це можна зробити за допомогою онлайн-валідаторів або інструментів розробника в браузерах.

- **Інструменти розробника**:
  `Chrome DevTools` - вбудований інструмент для розробників у браузері Google Chrome, який надає доступ до різних функцій відлагодження та аналізу веб-сторінок.
  Вкладки Elements, Console, Sources і Network дозволяють вивчати та редагувати HTML, CSS і JavaScript, переглядати консоль JavaScript, аналізувати мережеві запити та багато іншого.

---

**Корисні штуки та план кодування**:

- Перевірка вкладеності тегів:
  (https://caninclude.glitch.me/) (01:00)

- Атрибут `lang` - задає загальну мову сторінки, окремо вказуємо там де є посилання `href`, `alt` або текст:

```html
<section lang="ru">
  <h2 lang="uk">Привіт, світ!</h2>
  <p lang="uk">Це абзац написаний українською мовою.</p>
  <p>Это абзац написан на русском языке.</p>
</section>

<a href="english_page.html" lang="en">English Page</a>

<img src="example.jpg" alt="Привіт, світ!" lang="uk" />
````

- (https://realfavicongenerator.net/) (01:13)

- адресу бажано прописувати через `./` (відносна) - відносно файлу, де знаходимося (index.html) (01:21)

- `Figma` та структура сторінки (01:23)

- плагін "Emmet": (01:30)
  `ul>li\*5`  
  `header+main+footer`
  `section*8`

- `Logo` обгортаємо посиланням (01:40)

- `<h1>` - один на сторінку (01:47)

- інспектування елементів `Figma` (01:48)

- якірні посилання (скрол до відповідної секції на сторінці) (01:48)

- `nav` - навігаційне меню (посилання) (01:50)

- `ul` - об'єднаємо навігаційне меню за допомогою списку (01:50)

- багаторядковий курсор - затиснути `Alt` (01:51)

- фішка `Figma` - розносити блок тексту по різних меню (01:52)

- якірні посилання - (створюємо унікальні id-посилання) (01:53)

```html
<nav>
  <ul>
    <li><a href="#about">About</a></li>
    <li><a href="#price">Services and prices</a></li>
    <li><a href="#team">Barbers</a></li>
    <li><a href="#contacts">Contacts</a></li>
  </ul>
</nav>

<!-- Price section -->
<section id="price"></section>
```

- різниця між кнопками та посиланнями (01:59)

- безпечне посилання на зовнішні (сторонні) ресурси (02:03)

- Налаштування Pritier (02:38)
