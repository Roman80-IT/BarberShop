```html
<link rel="stylesheet" href="styles.css" type="text/css" media="all" />

<!-- Основний запис: -->
<link rel="stylesheet" href="styles.css" />
```

При підключенні CSS-файлу до HTML-документу найчастіше використовуються такі атрибути:

**rel:** вказує на відношення між поточним документом і пов'язаним ресурсом. Для підключення CSS використовують значення "stylesheet".

**href:** вказує на шлях до CSS-файлу.

**type:** вказує MIME-тип, який використовується для ресурсу. Для CSS це "text/css". Сьогодні цей атрибут зазвичай опускається, оскільки він за замовчуванням передбачається.

**media:** вказує, для яких пристроїв чи умов застосовуються стилі. Наприклад, "screen" для екранних пристроїв, "print" для принтерів або "all" для всіх пристроїв.

**title:** вказує назву стилів, яка може використовуватися при перемиканні між стилями.

**integrity:** використовується для забезпечення безпеки шляхом перевірки цілісності завантаженого ресурсу.

**crossorigin:** вказує, чи слід отримувати ресурс з підтримкою CORS.

## Пояснення атрибутів для тегу `<link>` в **HTML**:

| Атрибут       | Повна назва         | Опис                                                                          | Тег        | Можливі значення                                                                                                                                 |
| ------------- | ------------------- | ----------------------------------------------------------------------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| `rel`         | relationship        | Вказує на відношення між поточним документом і пов'язаним ресурсом            | `<link>`   | `"stylesheet"`, `"icon"`, `"preload"`, `"alternate"`, `"canonical"`, інші                                                                        |
|               |                     |                                                                               | `<a>`      | `"alternate"`, `"author"`, `"bookmark"`, `"help"`, `"license"`, `"next"`, `"nofollow"`, `"noopener"`, `"noreferrer"`, `"prev"`, `"search"`, інші |
| `href`        | hypertext reference | Вказує на шлях до пов'язаного ресурсу                                         | `<link>`   | URL до файлу або ресурсу                                                                                                                         |
|               |                     |                                                                               | `<a>`      | URL до файлу або ресурсу                                                                                                                         |
| `type`        | type                | Вказує MIME-тип пов'язаного ресурсу                                           | `<link>`   | `"text/css"`, `"application/rss+xml"`, `"application/atom+xml"`, інші                                                                            |
|               |                     |                                                                               | `<script>` | `"application/javascript"`, `"module"`, інші                                                                                                     |
| `media`       | media               | Вказує, для яких пристроїв чи умов застосовуються стилі                       | `<link>`   | `"all"`, `"screen"`, `"print"`, `"speech"`, медіа-запити, наприклад `"screen and (min-width: 600px)"`                                            |
|               |                     |                                                                               | `<style>`  | `"all"`, `"screen"`, `"print"`, `"speech"`, медіа-запити                                                                                         |
| `title`       | title               | Вказує назву стилів або документа                                             | `<link>`   | Будь-який текст                                                                                                                                  |
|               |                     |                                                                               | `<style>`  | Будь-який текст                                                                                                                                  |
| `integrity`   | integrity           | Використовується для забезпечення безпеки шляхом перевірки цілісності ресурсу | `<link>`   | Строка SRI (Subresource Integrity), яка містить хеш значення файлу                                                                               |
|               |                     |                                                                               | `<script>` | Строка SRI (Subresource Integrity), яка містить хеш значення файлу                                                                               |
| `crossorigin` | cross origin        | Вказує, чи слід отримувати ресурс з підтримкою CORS                           | `<link>`   | `"anonymous"`, `"use-credentials"`                                                                                                               |
|               |                     |                                                                               | `<script>` | `"anonymous"`, `"use-credentials"`                                                                                                               |

## Пояснення атрибутів для тега `<script>`

Ось таблиця з описом атрибутів тега `<script>` у HTML:

| Атрибут       | Тип      | Повна назва  | Опис                                                                                    | Можливі значення                                            |
| ------------- | -------- | ------------ | --------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| `src`         | URL      | source       | Вказує шлях до JavaScript-файлу                                                         | URL або шлях до файлу JS                                    |
| `type`        | MIME-тип | type         | Вказує MIME-тип JavaScript-файлу                                                        | `"text/javascript"`, `"module"`, `"application/json"`, інші |
| `defer`       | Boolean  | defer        | Вказує, що скрипт має бути виконаний після завантаження всього HTML-документу           | `"defer"` (опціонально)                                     |
| `async`       | Boolean  | asynchronous | Вказує, що скрипт має бути завантажений асинхронно і виконаний, як тільки завантажиться | `"async"` (опціонально)                                     |
| `integrity`   | Хеш      | integrity    | Використовується для перевірки цілісності JavaScript-файлу                              | Строка SRI (Subresource Integrity)                          |
| `crossorigin` | CORS     | cross origin | Вказує, чи слід отримувати ресурс з підтримкою CORS                                     | `"anonymous"`, `"use-credentials"`                          |

### Приклади використання атрибутів

#### Підключення JavaScript з атрибутом `src`:

```html
<script src="script.js" type="text/javascript"></script>

<!-- Підключення JavaScript з атрибутом defer: -->
<script src="script.js" type="text/javascript" defer></script>

<!-- Підключення JavaScript з атрибутом async: -->
<script src="script.js" type="text/javascript" async></script>

<!-- Підключення JavaScript з атрибутами integrity і crossorigin: -->
<script
  src="script.js"
  type="text/javascript"
  integrity="sha384-..."
  crossorigin="anonymous"
></script>
```

## Що таке MIME-тип?

**MIME-тип** (Multipurpose Internet Mail Extensions type) — це стандартний спосіб опису типу даних, які передаються через Інтернет.

### Структура MIME-типу

MIME-тип має формат `type/subtype`, де:

- **`type`** — основний тип даних.
- **`subtype`** — підкатегорія типу даних.

### Приклад MIME-типів

| MIME-тип                            | Опис                                  |
| ----------------------------------- | ------------------------------------- |
| `text/html`                         | HTML-документ                         |
| `text/css`                          | CSS-файл                              |
| `text/plain`                        | Простий текст                         |
| `application/javascript`            | JavaScript-файл                       |
| `application/json`                  | JSON-дані                             |
| `image/jpeg`                        | Зображення JPEG                       |
| `image/png`                         | Зображення PNG                        |
| `audio/mpeg`                        | Аудіофайл MP3                         |
| `video/mp4`                         | Відеофайл MP4                         |
| `application/xml`                   | XML-документ                          |
| `application/pdf`                   | PDF-файл                              |
| `application/x-www-form-urlencoded` | Дані з форм, закодовані в URL-форматі |

### Важливість MIME-типів

1. **Ідентифікація Типу Даних:**  
   MIME-типи допомагають серверам і браузерам визначити тип вмісту, який вони отримують або відправляють.

2. **Обробка Даних:**  
   Браузери та інші клієнти використовують MIME-типи для вибору правильного способу обробки даних.

3. **Передача Даних:**  
   MIME-типи є частиною заголовків HTTP-запитів і відповідей. Вони вказують, які дані передаються і як їх потрібно обробляти.

### Як вказати MIME-тип у HTML

#### Атрибут `type` у `<script>`

```html
<script src="script.js" type="text/javascript"></script>
```