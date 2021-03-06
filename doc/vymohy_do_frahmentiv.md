## Вимоги до текстів для БрУК

### Загальні вимоги

- оригінальні тексти (тобто неперекладні)
- мова материкової України (діаспорних авторів не беремо, навіть якщо їх видано в Україні, наприклад, Караванський)
- прозові тексти
- зредаговані (учнівський твір, приватний лист, особистий блог, чимало новинних текстів на pravda.com.ua не годяться)
- опубліковані (вперше) в 2010-2017рр. Твір, виданий 1975 року і перевиданий 2013 року, не підходить. Твір, написаний 1930 року і виданий (навіть уперше) без суттєвих змін 2013 року, не підходить, бо мова несучасна. З іншого боку, якщо автор писав свій твір впродовж 2005-2013 років і видав його 2013 року, - підходить. Сумнівні випадки обговорюємо або ігноруємо, якщо твори не принципові
- з одного джерела нам треба набрати тексту довжиною 2000 слововживань. З практики стало зрозуміло, що досить важко знайти якісний уривок такої довжини, тому можна/варто набирати цю кількість кількома фрагментами меншої довжини - 500-1000 слововживань, навіть 200-300, якщо це преса. Кожен такий фрагмент записуємо в окремий файл і в кінці назви додаємо _1, _2 тощо. Це особливо стосується преси і взагалі статей, бо там тексти загалом коротші. 
- кожен текст зберігаємо в окремому текстовому файлі в кодуванні UTF-8
- кожен текст має бути паспортизований (перелік метаданих нижче)

### Вимоги до якості текстів:

- без найменших ознак машинного чи людського перекладу (чимало текстів на pravda.com.ua та інших новинних сайтах цієї вимоги не задовольняють)
- фрагмент-кандидат спершу перевіряємо на наявність орфографічних і стилістичних помилок тут: http://r2u.org.ua/check - утилітою LanguageTool. Це дає змогу приблизно оцінити якість фрагмента, виявити поширені помилки (але виловлюються не всі!), а також на око оцінити якість тексту й знайти відносно "чисті" фрагменти. Ці фрагменти й варто опрацьовувати далі. Пропоновані з боку LT поправки слід враховувати (виносити в зону errors), але сприймати критично. Якщо фрагмент "пройшов відбір", треба вичитати його самостійно на предмет помилок:  
   - грамотність - відсутність орфографічних, пунктуаційних, граматичних помилок тощо
   - стиль - відсутність русизмів, активних дієприкметників, невдалих синтаксичних конструкцій (типу "План виконується нами")
   - порушення правил чергування і/й та у/в не виносимо в помилки, крім геть злісних випадків, коли вжитий прийменник звучить вкрай неприродно (на кшталт к/п/т/ф/х в с/т/п/к/х/н)
- кожен фрагмент треба вичитувати самому, щоб не було друкарських ляпів і стилістичних огріхів
- намагаємося підбирати тексти нешаблонні, жваві, розкуті, багаті лексикою, з влучними формулюваннями. Мова має бути поліфонічна. Не боїмося розмовної, жаргонної лексики, але без передозування. Вульгаризмів не треба.
- не беремо фрагментів, де є 50% і більше діалогу
- не беремо фрагментів, де багато слів, що імітують діалектну вимову. Наприклад, фрагмент зі стилізацією під діалектну вимову (скажімо, з В. Лиса) не підходить. 
- добираймо такі фрагменти, щоб їх і школярам можна було показувати. Наприклад, не варто брати фрагменти про інцест

### Зміни до фрагменту

- можна правити тільки геть очевидні друкарські помилки (наприклад, "водсю" на "водою"). Решту - виписувати в зону errors (див. нижче)
- виноски та посилання на літературні джерела з тексту забираємо ("стаття*", "виводить продукти обміну з організму [10]."); посилання на малюнки та таблиці залишаємо ("артезіанського басейну (табл. 1).")
- ставимо всюди українські лапки-ялиночки - ось такі `« »`
- фрагменти неодмінно треба переглядати в текстовому редакторі з увімкненими недрукованими знаками! Зокрема прибирати всі зайві проміжки, зайві пересення рядка тощо
- прибираємо знаки перенесення - уважно вичитуємо його в текстовому редакторі (щоб не було "при-хильність")

### Маркування окремих елементів

- якщо автор в тексті показує наголос, виділяючи слова/фрази курсивом, жирним шрифтом, підкресленням тощо, маркуємо таке за допомогою тега `<emphasis></emphasis>`. Інколи CAPSLOCK в тексті - це емфраза. Тоді пишемо ці слова звичайними літерами й додаємо подвійний тег `<emphasis></emphasis>`
- окрім випадків, описаних у попередньому пункті, маркуємо відповідними тегами слова чи шматки тексту, які в оригіналі йдуть курсивом чи жирним шрифтом: `<i>курсив</i>`, `<b>болд</b>`
- маркуємо формули, таблиці, діаграми, малюнки/рисунки одинарними тегом: `<formula>`, `<table>`, `<chart>`, `<picture>`
- шматки тексту іноземною мовою (наприклад, "Новости Донбасса") маркуємо тегом `<foreign></foreign>`. Якщо це українська транслітерація чужомовної назви/фрази ("Новості Донбасса"), тега не треба
- цитати маркуємо тегом `<quote></quote>`

### Джерела текстів

- електронні тексти з відкритих інтернет-джерел - газетні й журнальні публікації, уривки художньої та іншої літератури, наукові статті
- скани, викладені в інтернеті
- самі скануємо паперові видання (кілька сторінок), розпізнаємо й вичитуємо потрібної довжини фрагмент

__NB!__ Якщо беремо електронний текст видання (книжки), що в оригіналі є на папері, то варто вказувати місто й видавця. Дуже бажано знайти скан паперового варіанта, звірити електронний текст із друкованим виданням і вказати сторінки, з яких взято текст. Це додає достовірності й авторитетності всьому корпусу. Якщо ж скану немає, то вказуємо ел. ресурс, звідки взято текст, і обходимося без сторінок.

### Формат метаданих фрагменту тексту:

- `<id></id>` - ідентифікаційний номер фрагменту (латинська літера категорії - A, B, C...)
- `<author_surname></author_surname>- прізвище автора
- `<author_name></author_name>` - ім’я автора. Якщо авторів кілька, додаємо ідентифікатори: `<author_surname_1></author_surname_1>`, `<author_name_1></author_name_1>`, `<author_surname_2></author_surname_2>`, `<author_name_2></author_name_2>`
- `<title></title>` - назва твору, з якого взято фрагмент
- `<publ_in></publ_in>` - назва журналу/газети (якщо беремо журнальну/газетну статтю) чи книжки (якщо беремо окремий авторський твір із книжки)
- `<url></url>` - інтернет-адреса джерела (якщо беремо з електронного видання)
- `<publ_part></publ_part>` - число/том/випуск/частина друкованого видання, періодичного чи ні
- `<publ_place></publ_place>` - місце видання; для загальноукраїнських газет і журналів вказуємо "Київ"
- `<publisher></publisher>` - видавництво
- `<year></year>` - рік публікації
- `<pages></pages>` - номери сторінок, з яких узято фрагмент
- `<length></length>` - довжина в словах
- `<alt_orth></alt_orth>` - альтернативний правопис: ставимо 1, якщо правопис альтернативний ("любови", "ґрація"), ставимо 0, якщо офіційний
- `<errors></errors>` - тут описуємо помічені помилки за шаблоном "неправильне_слово - правильне_слово; ..." (помилки відокремлюємо крапкою з комою, не комою)
- `<comments></comments>` - коментарі (за потреби)
- `<body></body>` - сам фрагмент

__NB!__ Якщо якась інформація відсутня, залишаємо теги порожніми.

__NB!__ Послідовність цих тегів є незмінною для кожного фрагменту. Шаблон тегів беремо з [shablon_tagiv.txt](shablon_tagiv.txt).

__NB!__ Треба пильнувати, щоб вводити назву твору й окремо назву книжки. Наприклад, назва казки, з якої взято фрагмент, іде в зону `<title></title>`, а назва книжки "Казки лірника Сашка" - в зону `<publ_in></publ_in>`

__NB!__ Посилання на джерело типу `<url>http://toloka.hurtom.com</url>` не годиться. Посилання на інтернет-джерела даємо лише тоді, коли це сайт із повноцінною публікацією (переважно статтею). Якщо книжка в електронному форматі, то беремо pdf чи djvu й дивимося на сторінки, вказуємо вихідні дані паперового варіанта. Можна взяти якийсь суто текстовий е-формат, але тоді варто при нагоді звірити з паперовим виданням вихідну інформацію.

### Назва файлу

Назва файлу повинна складатись із категорії, прізвища автора, назви твору та року видання. Усі назви повинні бути написані латиницею. Назви зі статей з категорії "Преса" (A) повинні містити назву газети.

Зразки назви файлу:
- `A_gazeta.lviv.ua_Krystyniak_Na_leshchetakh_mov_na_krylakh_2014.txt`
- `D_Marynovych_Muzhnie priamostoiannia_2012.txt`
- `I_Herbish_1_Tepli_istoriyi_do_kavy_2012.txt`

### Категорії текстів у БрУК (відсотки визначено колективно 30.08.2014)

| Ідентифікатор | Категорія | Частка в корпусі | Опис текстів |
| ------------- |-----------|------------------|--------------|
| А | Преса | 25% | Репортажі, огляди, редакційні статті, листи до редакції; національні й регіональні видання; тематично - політика, спорт, суспільство, економіка й фінанси, короткі новини, культура - театр, література, музика, танці |
| B | Релігійна література | 3% | Книжки, періодика, брошури |
| С | Професійно-популярна література | 7% | Книжки й періодика; домоводство, ремесла, «сад і город», хобі, ремонт і будівництво, конструювання, музика й танці, домашні тварини, спорт, їжа й вино, подорожі, фермерство, робочі професії тощо |
| D | «Естетичні інформативні» тексти | 7% | Інформативні тексти, що не потрапляють в інші категорії, зокрема, біографії, мемуари, есеї, передмови, особисті листи, художня й мистецтвознавча критика, рекламні тексти |
| E | Адміністративні документи | 3% | Закони, урядові акти, звіти організацій/фондів/компаній, офіційні листи |
| F | Науково-популярна література | 5% | |
| G | Наукова література | 10% | Книжки й періодика; природничі й гуманітарні науки, техніка й інженерна справа |
| H | Навчальна література | 15% | Підручники, посібники, гуманітарні та природничі науки тощо |
| I | Художні тексти | 25% | Романи, повісті, оповідання, новели, за тематикою – загальна, детективи, фантастика, пригодницька, любовна, гумористична тощо |

Загалом тексти поділяються на два види – інформативні (призначені поінформувати читача) і художні (описують вигаданих персонажів і події). Інформативний вид охоплює категорії А-H, художній – лише I.
