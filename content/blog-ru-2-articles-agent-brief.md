# Задача для браузерного агента: сверстать 2 статьи блога «Алгоритм Дубай» в Тильде

## Кто ты и что делаешь

Ты работаешь в Тильде в проекте сайта **algorithmdubai.com** (образовательный центр «Алгоритм» в Дубае, русскоязычные дети 5,5-15 лет). Нужно опубликовать две новые статьи русского блога. Тексты, вёрстка, SEO-настройки и разметка уже готовы: ниже полный HTML-код каждой статьи. Твоя работа: создать страницы, вставить код, заполнить настройки, переименовать формы для CRM, опубликовать и проверить.

**Порядок важен:** сначала статья 1 («Как выбрать школу»), потом статья 2 («Подготовка к школе»), потому что статья 2 ссылается на статью 1.

## Как устроен блог сейчас

- Опубликованная статья-образец: **https://algorithmdubai.com/dubai_family_info_ru** («Жизнь в Дубае с детьми: гид для родителей»). Структура страницы сверху вниз:
  1. меню (русское);
  2. блок с заголовком статьи (H1) и подписью;
  3. блок **T123 «HTML-код»** с самой статьёй (стили, текст, картинки, FAQ, разметка schema.org уже внутри кода);
  4. попапы `#reg` («Запись на подбор программы») и `#trial`, красная форма «Запишитесь на консультацию и диагностику»;
  5. FAQ центра, контакты, подвал.
- Хаб блога: **https://algorithmdubai.com/blog-ru**, на нём карточка гида с кнопкой «Читать».
- Кнопка в статье `href="#reg"` открывает попап записи, ссылки `/dia`, `/preparatory`, `/weekends`, `/5days`, `/courses` ведут на продуктовые страницы.

## Пошагово для каждой статьи

1. В проекте Тильды найди страницу **dubai_family_info_ru** и сделай её **копию** (Дублировать страницу). Работай только с копией, оригинал не меняй.
2. Открой копию. В блоке с заголовком (H1) замени текст заголовка на H1 из карточки статьи ниже. Убедись, что у этого текста тег **H1** (в настройках элемента/блока). Других H1 на странице быть не должно.
3. Найди блок **T123 «HTML-код»** со статьёй-гидом. Открой «Контент» блока, **полностью удали** старый код и вставь код статьи из раздела ниже целиком, от первой строки `<!--` до последней `</script>`. Сохрани.
4. **Настройки страницы → Главное:**
   - Заголовок (title) и Описание (description): из карточки статьи;
   - Адрес страницы: из карточки (латиница, без слеша в начале).
5. **Настройки страницы → Соцсети:** заголовок и описание из карточки, картинка: скачай по ссылке «Картинка для соцсетей» и загрузи.
6. **Настройки страницы → SEO/индексация:** снят запрет индексации (страница должна индексироваться).
7. **Формы для CRM.** На странице есть попап `#reg`, попап `#trial` и красная форма консультации. В каждой форме открой «Контент» → поля → скрытые поля (hidden) и задай значения из карточки статьи:
   - скрытое поле `formname` и одноимённое название формы;
   - скрытое поле `programs`: такое же значение, как formname.
   Получатели данных (интеграции с CRM) **не трогай**.
8. Блоки ниже статьи (FAQ центра, контакты, подвал) оставь как в гиде.
9. Нажми **Опубликовать**.
10. Открой опубликованную страницу и проверь пункты из раздела «Проверка».
11. На странице **blog-ru** продублируй карточку гида и замени: картинку, заголовок, текст и ссылку кнопки «Читать» на данные карточки для хаба. Опубликуй blog-ru.

## Чего не делать

- Не менять оригинальную страницу dubai_family_info_ru и другие страницы сайта, кроме blog-ru.
- Не редактировать текст внутри HTML-кода статьи: он вычитан и проверен.
- Не менять получателей данных у форм и настройки проекта.
- Не добавлять второй H1 и не дублировать статью в других блоках.

## Проверка после публикации

- Адрес открывается, H1 правильный и один.
- Внутри статьи видны картинки, таблица, оглавление, раскрывающиеся частые вопросы.
- Ссылки «Записаться на диагностику», «Подготовка к школе», карточки программ ведут на /dia, /preparatory, /weekends, /5days.
- Кнопка «Записаться на консультацию» в конце статьи открывает попап записи.
- В исходном коде страницы title и description совпадают с карточкой.
- Тестовую заявку **не отправлять**.

---

## Статья 1. Как выбрать школу в Дубае

| Поле | Значение |
|---|---|
| Название страницы в Тильде | Блог RU: Как выбрать школу в Дубае |
| Адрес страницы | `kak-vybrat-shkolu-v-dubae` |
| H1 (заголовок в блоке над статьёй) | Как выбрать школу в Дубае: программы, рейтинг KHDA и поступление |
| Title | `Как выбрать школу в Дубае: программы, KHDA, поступление` |
| Description | `Британская, американская или IB? Как читать рейтинг KHDA, какие документы нужны, сколько стоит депозит и как подготовить русскоязычного ребёнка к школе в Дубае.` |
| Соцсети: заголовок | Как выбрать школу в Дубае: пошаговый план для родителей |
| Соцсети: описание | Программы, рейтинг KHDA, документы, депозит и вступительный тест. Гид от центра «Алгоритм». |
| Картинка для соцсетей | https://algorithmdubai-production.up.railway.app/blog-images/classroom-pupils-at-desks.webp |
| formname и programs, попап #reg | `Блог ру школа: подбор программы` |
| formname и programs, попап #trial | `Блог ру школа: пробный урок` |
| formname и programs, красная форма | `Блог ру школа: консультация и диа` |
| Карточка на blog-ru: заголовок | Как выбрать школу в Дубае |
| Карточка на blog-ru: текст | Британская, американская или IB, рейтинг KHDA, документы и поступление |
| Карточка на blog-ru: картинка | https://algorithmdubai-production.up.railway.app/blog-images/classroom-pupils-at-desks.webp |
| Карточка на blog-ru: ссылка | `https://algorithmdubai.com/kak-vybrat-shkolu-v-dubae` |

### HTML-код статьи 1 (вставить целиком в блок T123)

```html
<!-- Алгоритм Дубай · Как выбрать школу в Дубае (RU) · вставить в блок T123 «HTML-код» на странице /kak-vybrat-shkolu-v-dubae -->
<style>
.alg-art{--brand:#9e2744;--coral:#e1625c;--pink:#fee5e4;--ink:#1f1818;--grey:#494949;--line:#ecdfe2;
 font-family:var(--t-text-font,'Open Sans'),Arial,sans-serif;color:var(--ink);font-size:18px;line-height:1.65;
 max-width:820px;margin:0 auto;padding:8px 20px 72px;box-sizing:border-box}
.alg-art *{box-sizing:border-box}
.alg-art h2,.alg-art h3{font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;color:var(--ink);line-height:1.25}
.alg-art h2{font-size:32px;font-weight:700;margin:64px 0 18px;padding-top:24px;border-top:2px solid var(--pink);scroll-margin-top:90px}
.alg-art h3{font-size:22px;font-weight:700;margin:36px 0 10px}
.alg-art p{margin:0 0 16px}
.alg-art a{color:var(--brand);text-decoration:underline;text-underline-offset:3px}
.alg-art a:hover{color:var(--coral)}
.alg-art ul,.alg-art ol{margin:0 0 18px;padding-left:24px}
.alg-art li{margin-bottom:6px}
.alg-art ul li::marker{color:var(--brand)}
.alg-art ol li::marker{color:var(--brand);font-weight:700}
.alg-byline{font-size:15px;color:var(--grey);margin:0 0 24px;line-height:2}
.alg-byline span{background:var(--pink);color:var(--brand);border-radius:999px;padding:3px 12px;font-weight:600;margin-right:10px}
.alg-lead{font-size:20px;color:var(--ink)}
.alg-toc{background:#fff7f6;border:1px solid var(--line);border-radius:20px;padding:24px 28px;margin:28px 0 8px}
.alg-toc b{display:block;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-size:14px;letter-spacing:.08em;text-transform:uppercase;color:var(--brand);margin-bottom:12px}
.alg-toc ol{columns:2;column-gap:32px;margin:0;padding-left:22px}
.alg-toc a{text-decoration:none;color:var(--ink)}
.alg-toc a:hover{color:var(--brand)}
.alg-note{background:var(--pink);border-left:5px solid var(--brand);border-radius:14px;padding:18px 22px;margin:22px 0}
.alg-note p:last-child{margin:0}
.alg-promo{background:var(--brand);color:#fff;border-radius:20px;padding:26px 28px;margin:30px 0}
.alg-promo p{margin:0 0 14px}
.alg-promo a{color:#fff}
.alg-promo .alg-btn{background:#fff;color:var(--brand)!important}
.alg-btn{display:inline-block;background:var(--brand);color:#fff!important;text-decoration:none!important;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:600;font-size:16px;border-radius:12px;padding:13px 26px;transition:opacity .2s}
.alg-btn:hover{opacity:.88}
.alg-cards{display:grid;grid-template-columns:repeat(2,1fr);gap:14px;margin:18px 0 22px}
.alg-card{border:1px solid var(--line);border-radius:16px;padding:18px 20px;background:#fff;font-size:16px;line-height:1.55}
.alg-card a{display:block;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:700;font-size:17px;text-decoration:none;margin-bottom:6px;color:var(--ink)}
.alg-card a:hover{color:var(--brand)}
.alg-card a::after{content:" ↗";color:var(--brand);font-weight:400}
.alg-art .alg-steps{list-style:none;padding:0;counter-reset:s}
.alg-steps li{counter-increment:s;position:relative;padding:4px 0 10px 52px;margin:0}
.alg-steps li::before{content:counter(s);position:absolute;left:0;top:0;width:36px;height:36px;border-radius:50%;background:var(--brand);color:#fff;font-weight:700;display:flex;align-items:center;justify-content:center;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif}
.alg-table{width:100%;border-collapse:separate;border-spacing:0;margin:18px 0 24px;font-size:16px;border:1px solid var(--line);border-radius:14px;overflow:hidden}
.alg-table th{background:var(--brand);color:#fff;text-align:left;padding:12px 14px;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:600}
.alg-table td{padding:12px 14px;border-top:1px solid var(--line);vertical-align:top}
.alg-table tr:nth-child(even) td{background:#fff7f6}
.alg-faq details{border:1px solid var(--line);border-radius:14px;margin:0 0 10px;background:#fff}
.alg-faq summary{cursor:pointer;list-style:none;padding:16px 52px 16px 20px;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:600;font-size:17px;position:relative}
.alg-faq summary::-webkit-details-marker{display:none}
.alg-faq summary::after{content:"+";position:absolute;right:20px;top:50%;transform:translateY(-50%);font-size:26px;color:var(--brand);font-weight:400}
.alg-faq details[open] summary::after{content:"–"}
.alg-faq details p{padding:0 20px 16px;margin:0}
.alg-sources{font-size:15px;color:var(--grey)}
.alg-final{text-align:center;background:#fff7f6;border-radius:20px;padding:34px 24px;margin-top:48px}
.alg-final p{font-size:19px;margin-bottom:18px}
.alg-fig{margin:26px 0 30px}
.alg-fig img{display:block;width:100%;height:auto;aspect-ratio:16/9;object-fit:cover;border-radius:20px}
.alg-fig figcaption{font-size:14px;color:var(--grey);margin-top:10px;text-align:center}
.alg-duo{display:grid;grid-template-columns:1fr 1fr;gap:14px}
.alg-duo img{aspect-ratio:4/3}
.alg-duo figcaption{grid-column:1/-1;margin-top:0}
.alg-tl{display:flex;gap:0;margin:26px 0 30px;position:relative}
.alg-tl-item{flex:1;position:relative;padding:44px 10px 0;text-align:center;font-size:15px;line-height:1.45}
.alg-tl-item::before{content:"";position:absolute;top:15px;left:0;right:0;height:3px;background:var(--pink)}
.alg-tl-item:first-child::before{left:50%}.alg-tl-item:last-child::before{right:50%}
.alg-tl-item::after{content:"";position:absolute;top:6px;left:50%;transform:translateX(-50%);width:21px;height:21px;border-radius:50%;background:var(--brand);box-shadow:0 0 0 5px #fff}
.alg-tl-item b{display:block;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;color:var(--brand);font-size:16px;margin-bottom:4px}
.alg-ages{display:flex;align-items:flex-end;gap:12px;margin:24px 0 30px;height:300px}
.alg-age{flex:1;border-radius:16px 16px 6px 6px;background:var(--pink);padding:14px 12px;display:flex;flex-direction:column;justify-content:flex-start;font-size:14px;line-height:1.4}
.alg-age b{font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-size:17px;color:var(--brand);margin-bottom:4px}
.alg-age:nth-child(1){height:52%}.alg-age:nth-child(2){height:68%}.alg-age:nth-child(3){height:84%}
.alg-age:nth-child(4){height:100%;background:var(--brand);color:#fff}.alg-age:nth-child(4) b{color:#fff}
.alg-khda{display:grid;grid-template-columns:repeat(6,1fr);gap:6px;margin:20px 0 8px}
.alg-khda div{border-radius:10px;padding:14px 6px;text-align:center;color:#fff;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:600;font-size:14px;line-height:1.25}
.alg-khda-cap{display:flex;justify-content:space-between;font-size:13px;color:var(--grey);margin-bottom:26px}
@media (max-width:640px){
 .alg-art{font-size:16px;padding:0 16px 56px}
 .alg-lead{font-size:18px}
 .alg-art h2{font-size:25px;margin-top:48px}
 .alg-art h3{font-size:19px}
 .alg-toc{padding:20px}
 .alg-toc ol{columns:1}
 .alg-cards{grid-template-columns:1fr}
 .alg-table{font-size:14px}
 .alg-table th,.alg-table td{padding:10px}
 .alg-tl{flex-direction:column;gap:0}
 .alg-tl-item{text-align:left;padding:0 0 18px 40px}
 .alg-tl-item::before{top:0;bottom:0;left:10px;right:auto;width:3px;height:auto}
 .alg-tl-item:first-child::before{left:10px;top:12px}.alg-tl-item:last-child::before{right:auto;bottom:auto;height:12px}
 .alg-tl-item::after{top:2px;left:0;transform:none}
 .alg-ages{height:auto;flex-direction:column;align-items:stretch}
 .alg-age{height:auto!important;border-radius:14px}
 .alg-khda{grid-template-columns:repeat(3,1fr)}
 .alg-fig img{border-radius:14px}
 .alg-duo{gap:8px}
}
.alg-card b{display:block;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:700;font-size:17px;color:var(--brand);margin-bottom:8px}
.alg-card ul{margin:0;padding-left:20px}
.alg-card li{margin-bottom:4px}
</style>

<article class="alg-art" lang="ru" itemscope itemtype="https://schema.org/Article">
<meta itemprop="headline" content="Как выбрать школу в Дубае: программы, рейтинг KHDA и поступление">

<p class="alg-byline"><span>Гид для родителей</span> Команда образовательного центра «Алгоритм» · Обновлено <time datetime="2026-11-26">26 ноября 2026</time></p>

<p class="alg-lead">От школы в Дубае зависит многое: на каком языке ребёнок будет думать через пару лет, в какие университеты сможет поступать и с кем будет дружить. Выбор при этом огромный: в эмирате работают сотни частных школ с десятком разных программ.</p>

<p>Ниже порядок действий, который помогает семьям нашего центра сузить выбор до 2-3 школ и спокойно пройти поступление.</p>

<figure class="alg-fig"><img src="https://algorithmdubai-production.up.railway.app/blog-images/classroom-pupils-at-desks.webp" alt="Ученики слушают учителя за партами в светлом классе" width="960" height="540"><figcaption>Сначала выбирают программу, потом конкретную школу</figcaption></figure>

<nav class="alg-toc" aria-label="Содержание">
<b>Содержание</b>
<ol>
<li><a href="#program">Выберите программу</a></li>
<li><a href="#khda">Посмотрите рейтинг KHDA</a></li>
<li><a href="#practical">Учтите дорогу и расходы</a></li>
<li><a href="#tour">Съездите на экскурсию</a></li>
<li><a href="#documents">Подготовьте документы</a></li>
<li><a href="#assessment">Пройдите тестирование</a></li>
<li><a href="#prepare">Как подготовить ребёнка</a></li>
<li><a href="#russian">Как сохранить русский</a></li>
<li><a href="#faq">Частые вопросы</a></li>
</ol>
</nav>

<h2 id="program">Шаг 1. Решите, какая программа нужна ребёнку</h2>
<p>Программа важнее названия школы. От неё зависят экзамены, нагрузка и то, в какие университеты ребёнку будет проще поступать.</p>

<table class="alg-table">
<thead><tr><th>Программа</th><th>Итоговые экзамены</th><th>Кому подходит</th></tr></thead>
<tbody>
<tr><td><b>Британская</b></td><td>IGCSE в 16 лет, A-Level в 18 лет</td><td>Тем, кто смотрит на вузы Великобритании и Европы и любит понятную систему с экзаменами</td></tr>
<tr><td><b>Американская</b></td><td>High School Diploma и средний балл GPA, для вузов США плюс SAT или ACT</td><td>Тем, кто планирует учёбу в США или Канаде и лучше работает равномерно в течение года</td></tr>
<tr><td><b>IB</b></td><td>Диплом IB после двух последних лет (DP)</td><td>Самостоятельным детям: много проектов, эссе и исследований, диплом признают вузы по всему миру</td></tr>
</tbody>
</table>

<h3>Британская программа</h3>
<p>Самая распространённая в Дубае. Обучение делится на ступени (Key Stages). В 16 лет ученики сдают IGCSE, в 18 лет A-Level. Эти экзамены принимают британские и многие другие университеты.</p>

<h3>Американская программа</h3>
<p>Широкий выбор предметов и накопительная система оценок (GPA), в конце выдают High School Diploma. Для поступления в американские вузы дополнительно сдают SAT или ACT.</p>

<h3>Программа IB</h3>
<p>International Baccalaureate состоит из трёх ступеней: PYP в начальной школе, MYP в средней и DP в последние два года. Диплом IB признают университеты по всему миру. Программа считается одной из самых нагруженных: много исследовательских проектов, эссе и самостоятельной работы.</p>

<h3>Другие варианты</h3>
<p>В Дубае есть школы с индийской (CBSE, ICSE), французской, немецкой и другими национальными программами. Школ с полной российской программой здесь мало. Поэтому русскоязычные семьи чаще выбирают международную школу, а российскую программу поддерживают параллельно.</p>

<h2 id="khda">Шаг 2. Посмотрите рейтинг школы в KHDA</h2>
<p>Частные школы Дубая контролирует KHDA (Knowledge and Human Development Authority). По итогам инспекции школа получает общую оценку по шкале из шести уровней:</p>

<div class="alg-khda" role="list" aria-label="Шкала рейтинга школ KHDA">
<div role="listitem" style="background:#1f7a4d">Outstanding</div><div role="listitem" style="background:#4c9a5a">Very Good</div><div role="listitem" style="background:#8bb54a">Good</div><div role="listitem" style="background:#d9a52b">Acceptable</div><div role="listitem" style="background:#e1625c">Weak</div><div role="listitem" style="background:#9e2744">Very Weak</div>
</div>
<div class="alg-khda-cap"><span>Высшая оценка</span><span>Низшая оценка</span></div>

<p>Инспекторы смотрят на успеваемость, качество преподавания, безопасность, работу с детьми с особыми потребностями, уровень арабского языка и исламских исследований.</p>

<div class="alg-note">
<p>В 2024-25 и 2025-26 учебных годах KHDA не проводила плановых инспекций большинства школ, поэтому у них действует оценка с последней проверки. Помимо итоговой оценки на странице школы в справочнике KHDA есть краткий отчёт для родителей (parent summary): в нём видно, как школа работает с преподаванием и благополучием детей.</p>
</div>

<p>Как пользоваться рейтингом:</p>
<ul>
<li><b>Читайте отчёт, а не только итоговую оценку.</b> Английский в школе может быть на уровне Outstanding, а математика на уровне Good.</li>
<li><b>Смотрите динамику.</b> Школа, которая выросла с Good до Very Good, бывает интереснее той, что годами держит одну оценку.</li>
<li><b>Рейтинг не заменяет визит.</b> Он не покажет атмосферу, отношение учителей и то, как школа помогает детям, для которых английский второй язык.</li>
</ul>
<p>Рейтинги и отчёты публикуются на сайте KHDA и в его приложении.</p>

<h2 id="practical">Шаг 3. Учтите дорогу и расходы</h2>
<p><b>Дорога.</b> Дубай большой, и школа в 40 минутах езды превращается почти в полтора часа в машине каждый день. Спросите, ходит ли школьный автобус в ваш район.</p>
<p><b>Стоимость.</b> Плата за обучение сильно отличается от школы к школе и растёт с каждым классом. Кроме самой учёбы (tuition fee) заложите в бюджет вступительный взнос, депозит, форму, транспорт, питание и кружки. Актуальные цены публикуют сами школы.</p>
<p><b>Поддержка английского.</b> Если ребёнок только переехал, спросите про программу EAL (English as an Additional Language): как она устроена, сколько часов в неделю и когда ребёнка переводят в обычный поток.</p>
<p><b>Русскоязычные дети в классе.</b> В первые месяцы с ними легче адаптироваться. Но если их слишком много, английский может развиваться медленнее.</p>

<h2 id="tour">Шаг 4. Съездите на экскурсию</h2>
<p>Выберите 3-5 школ и запишитесь на school tour. Вопросы, которые стоит задать:</p>
<ul>
<li>Сколько детей в классе и сколько помощников у учителя?</li>
<li>Как школа работает с детьми, которые пока плохо говорят по-английски?</li>
<li>Как часто родители получают обратную связь?</li>
<li>Какие кружки входят в стоимость, а какие оплачиваются отдельно?</li>
<li>Есть ли места в нужном классе и есть ли лист ожидания?</li>
</ul>
<p>Посмотрите, как учителя общаются с детьми в коридорах. Это говорит о школе больше, чем презентация приёмной комиссии.</p>

<figure class="alg-fig"><img src="https://algorithmdubai-production.up.railway.app/blog-images/russian-class-girl-at-desk.webp" alt="Девочка улыбается за партой на уроке" width="960" height="540" loading="lazy"><figcaption>На экскурсии смотрите, как учителя общаются с детьми</figcaption></figure>

<h2 id="documents">Шаг 5. Подготовьте документы</h2>
<p>Набор зависит от школы, но обычно нужны:</p>
<ul>
<li>заявка (online application) и вступительный взнос;</li>
<li>паспорта ребёнка и родителей;</li>
<li>резидентская виза и Emirates ID: для подачи заявки можно без них, для начала учёбы они обязательны;</li>
<li>свидетельство о рождении;</li>
<li>фотографии;</li>
<li>табели и характеристики из прежней школы за последние 1-2 года;</li>
<li>справка о прививках;</li>
<li>трансферный сертификат (Transfer Certificate) из прежней школы.</li>
</ul>
<div class="alg-note">
<p>Трансферный сертификат обязателен для детей, которые идут в Year 3 (Grade 2) и старше из школы за пределами Дубая. Если документ выдан за границей, его заверяют в стране выдачи и в посольстве ОАЭ. Без него ребёнка не допустят к занятиям, поэтому точный порядок уточните в выбранной школе заранее.</p>
</div>
<p>Документы на русском языке обычно нужно перевести на английский или арабский.</p>

<h2 id="assessment">Шаг 6. Пройдите вступительное тестирование</h2>
<ol class="alg-steps">
<li>Вы подаёте заявку и платите вступительный взнос. По правилам KHDA он не превышает 500 AED и не засчитывается в оплату обучения.</li>
<li>Ребёнок проходит assessment: тест по английскому и математике, иногда собеседование. Для младших это игровая встреча, для старших письменный тест.</li>
<li>Если всё хорошо, школа присылает предложение о зачислении (offer).</li>
<li>Чтобы закрепить место, вы вносите депозит. KHDA ограничивает его 10% от годовой стоимости обучения, потом он засчитывается в оплату.</li>
</ol>
<p>Многие школы принимают детей в течение всего года, если в классе есть места. Но в популярные школы очередь собирается за год и больше, поэтому начинайте заранее.</p>

<h3>Возраст при поступлении</h3>
<p>С 2026-27 учебного года для детей, которые впервые поступают в школу Дубая, класс определяют по возрасту на 31 декабря. В школах, где учебный год начинается в сентябре, это FS1 с 3 лет, FS2 с 4 лет, Year 1 с 5 лет и Year 2 с 6 лет.</p>

<h2 id="prepare">Как подготовить ребёнка к поступлению</h2>
<p>Русскоязычные дети чаще спотыкаются не на математике, а на английском: не понимают формулировку задания или теряются в незнакомом формате теста.</p>
<p>Что помогает:</p>
<ol>
<li><b>Оценить уровень заранее,</b> за полгода до поступления, а не за месяц.</li>
<li><b>Тренировать формат теста</b>, а не только язык: задания с картинками, логические задачи, чтение коротких текстов на время.</li>
<li><b>Держать математику на сильном уровне.</b> Российская программа обычно даёт хорошую базу, и на тесте это реальное преимущество.</li>
</ol>
<p>В «Алгоритме» английский ведут педагоги-носители языка. Все направления собраны на странице <a href="/courses">курсов для детей</a>.</p>

<div class="alg-promo">
<p>Не уверены, на каком уровне сейчас английский и русский у ребёнка? Запишитесь на бесплатную диагностику: педагог оценит знания и подскажет, с чего начать подготовку.</p>
<a class="alg-btn" href="/dia">Записаться на диагностику</a>
</div>

<h2 id="russian">Как не потерять русский язык и российскую программу</h2>
<p>Международная школа почти всегда вытесняет русский. Через 1-2 года ребёнок говорит по-русски, но читать и писать ему уже трудно. Если для семьи важно сохранить язык или оставить возможность вернуться в российскую школу, программу нужно поддерживать параллельно.</p>
<div class="alg-cards">
<div class="alg-card"><a href="/weekends">Российская программа для учеников международных школ</a>1-8 классы, очно по пятницам или субботам и онлайн-уроки в будни. Промежуточные аттестации проходят без поездок в Москву.</div>
<div class="alg-card"><a href="/5days">Пятидневная российская программа</a>Очно с понедельника по пятницу, 1-4 классы. Подходит тем, кто хочет учиться по российской программе в Дубае.</div>
<div class="alg-card"><a href="/dia">Бесплатная диагностика</a>Покажет, на каком уровне сейчас русский язык и школьные предметы.</div>
<div class="alg-card"><a href="/dubai_family_info_ru">Гид «Жизнь в Дубае с детьми»</a>Роды, детский сад, школа, няня и досуг в одной статье.</div>
</div>

<h2 id="faq">Частые вопросы</h2>
<div class="alg-faq">
<details><summary>Сколько стоит школа в Дубае?</summary><p>Стоимость зависит от школы, программы и класса и может отличаться в несколько раз. Смотрите цены на сайтах школ и закладывайте дополнительные расходы: вступительный взнос, депозит, форму и транспорт.</p></details>
<details><summary>Когда подавать документы в школу в Дубае?</summary><p>В популярные школы за год и раньше. Многие школы принимают детей и в течение года, если есть места, но выбор тогда меньше.</p></details>
<details><summary>Какой рейтинг KHDA считается хорошим?</summary><p>Outstanding и Very Good это высший уровень, Good уверенный средний. Читайте полный отчёт: общая оценка не показывает сильные и слабые стороны по предметам.</p></details>
<details><summary>Есть ли в Дубае русская школа?</summary><p>Школ с полной российской программой в Дубае мало. Многие семьи выбирают международную школу и параллельно учатся по российской программе, например в гибридном формате с аттестациями в Дубае.</p></details>
<details><summary>Нужен ли английский для поступления?</summary><p>Да, почти везде проводят тест по английскому. Если уровень пока слабый, ищите школы с программой EAL и начинайте подготовку заранее.</p></details>
<details><summary>Какой депозит берут школы при зачислении?</summary><p>По правилам KHDA вступительный взнос не больше 500 AED, а депозит за место не больше 10% от годовой стоимости обучения. Депозит потом засчитывается в оплату.</p></details>
</div>

<h2 id="sources">Источники</h2>
<div class="alg-sources">
<p>Правила в ОАЭ меняются, поэтому перед подачей документов сверяйтесь с официальными источниками:</p>
<ul>
<li><a href="https://web.khda.gov.ae/en/Guides/Parents/A-Parent%E2%80%99s-Guide-to-Fees,-Deposits-and-Refunds-(1)?utm_source=algorithmdubai&utm_medium=referral&utm_campaign=blog_school" target="_blank" rel="noopener">KHDA</a>: правила о взносах, депозитах и возвратах в частных школах Дубая;</li>
<li><a href="https://web.khda.gov.ae/en/About-Us/News/2025/KHDA-announces-pause-on-school-inspections-for-202?utm_source=algorithmdubai&utm_medium=referral&utm_campaign=blog_school" target="_blank" rel="noopener">KHDA</a>: пауза в инспекциях школ;</li>
<li><a href="https://www.khaleejtimes.com/uae/dubai-school-admissions-khda-new-guide-age-cut-off?utm_source=algorithmdubai&utm_medium=referral&utm_campaign=blog_school" target="_blank" rel="noopener">Khaleej Times</a>: новые возрастные правила приёма с 2026-27 учебного года.</li>
</ul>
</div>

<div class="alg-final">
<p>Образовательный центр «Алгоритм» в Дубае: подготовка к школе, российская программа для учеников международных школ, курсы русского и английского языка.</p>
<a class="alg-btn" href="#reg">Записаться на консультацию</a>
</div>
</article>

<script type="application/ld+json">
{
 "@context": "https://schema.org",
 "@graph": [
  {
   "@type": "Article",
   "headline": "Как выбрать школу в Дубае: программы, рейтинг KHDA и поступление",
   "description": "Британская, американская или IB? Как читать рейтинг KHDA, какие документы нужны, сколько стоит депозит и как подготовить русскоязычного ребёнка к школе в Дубае.",
   "inLanguage": "ru",
   "datePublished": "2026-11-26",
   "dateModified": "2026-11-26",
   "mainEntityOfPage": "https://algorithmdubai.com/kak-vybrat-shkolu-v-dubae",
   "image": "https://algorithmdubai-production.up.railway.app/blog-images/classroom-pupils-at-desks.webp",
   "author": {
    "@type": "Organization",
    "name": "Образовательный центр «Алгоритм»",
    "url": "https://algorithmdubai.com/ru"
   },
   "publisher": {
    "@type": "Organization",
    "name": "Образовательный центр «Алгоритм»",
    "url": "https://algorithmdubai.com/ru"
   }
  },
  {
   "@type": "BreadcrumbList",
   "itemListElement": [
    {
     "@type": "ListItem",
     "position": 1,
     "name": "Главная",
     "item": "https://algorithmdubai.com/ru"
    },
    {
     "@type": "ListItem",
     "position": 2,
     "name": "Блог",
     "item": "https://algorithmdubai.com/blog-ru"
    },
    {
     "@type": "ListItem",
     "position": 3,
     "name": "Как выбрать школу в Дубае",
     "item": "https://algorithmdubai.com/kak-vybrat-shkolu-v-dubae"
    }
   ]
  },
  {
   "@type": "FAQPage",
   "mainEntity": [
    {
     "@type": "Question",
     "name": "Сколько стоит школа в Дубае?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Стоимость зависит от школы, программы и класса и может отличаться в несколько раз. Смотрите цены на сайтах школ и закладывайте дополнительные расходы: вступительный взнос, депозит, форму и транспорт."
     }
    },
    {
     "@type": "Question",
     "name": "Когда подавать документы в школу в Дубае?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "В популярные школы за год и раньше. Многие школы принимают детей и в течение года, если есть места, но выбор тогда меньше."
     }
    },
    {
     "@type": "Question",
     "name": "Какой рейтинг KHDA считается хорошим?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Outstanding и Very Good это высший уровень, Good уверенный средний. Читайте полный отчёт: общая оценка не показывает сильные и слабые стороны по предметам."
     }
    },
    {
     "@type": "Question",
     "name": "Есть ли в Дубае русская школа?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Школ с полной российской программой в Дубае мало. Многие семьи выбирают международную школу и параллельно учатся по российской программе, например в гибридном формате с аттестациями в Дубае."
     }
    },
    {
     "@type": "Question",
     "name": "Нужен ли английский для поступления?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Да, почти везде проводят тест по английскому. Если уровень пока слабый, ищите школы с программой EAL и начинайте подготовку заранее."
     }
    },
    {
     "@type": "Question",
     "name": "Какой депозит берут школы при зачислении?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "По правилам KHDA вступительный взнос не больше 500 AED, а депозит за место не больше 10% от годовой стоимости обучения. Депозит потом засчитывается в оплату."
     }
    }
   ]
  }
 ]
}
</script>
```

---

## Статья 2. Подготовка к школе в Дубае

| Поле | Значение |
|---|---|
| Название страницы в Тильде | Блог RU: Подготовка к школе в Дубае |
| Адрес страницы | `podgotovka-k-shkole-v-dubae` |
| H1 (заголовок в блоке над статьёй) | Подготовка к школе в Дубае: что должен уметь ребёнок в 5-6 лет |
| Title | `Подготовка к школе в Дубае: что должен уметь ребёнок` |
| Description | `Чек-лист готовности к школе для детей 5-6 лет: речь, чтение, счёт, английский, внимание и самостоятельность. Как готовить ребёнка к российской и международной школе.` |
| Соцсети: заголовок | Что должен уметь ребёнок к школе: чек-лист для родителей в Дубае |
| Соцсети: описание | Речь, чтение, счёт, английский и самостоятельность. Как готовиться к российской и международной школе. |
| Картинка для соцсетей | https://algorithmdubai-production.up.railway.app/blog-images/kids-shapes-activity-with-parents.webp |
| formname и programs, попап #reg | `Блог ру подготовка: подбор программы` |
| formname и programs, попап #trial | `Блог ру подготовка: пробный урок` |
| formname и programs, красная форма | `Блог ру подготовка: консультация и диа` |
| Карточка на blog-ru: заголовок | Подготовка к школе в Дубае |
| Карточка на blog-ru: текст | Чек-лист готовности к школе для детей 5-6 лет и привычки для дома |
| Карточка на blog-ru: картинка | https://algorithmdubai-production.up.railway.app/blog-images/kids-shapes-activity-with-parents.webp |
| Карточка на blog-ru: ссылка | `https://algorithmdubai.com/podgotovka-k-shkole-v-dubae` |

### HTML-код статьи 2 (вставить целиком в блок T123)

```html
<!-- Алгоритм Дубай · Подготовка к школе в Дубае (RU) · вставить в блок T123 «HTML-код» на странице /podgotovka-k-shkole-v-dubae -->
<style>
.alg-art{--brand:#9e2744;--coral:#e1625c;--pink:#fee5e4;--ink:#1f1818;--grey:#494949;--line:#ecdfe2;
 font-family:var(--t-text-font,'Open Sans'),Arial,sans-serif;color:var(--ink);font-size:18px;line-height:1.65;
 max-width:820px;margin:0 auto;padding:8px 20px 72px;box-sizing:border-box}
.alg-art *{box-sizing:border-box}
.alg-art h2,.alg-art h3{font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;color:var(--ink);line-height:1.25}
.alg-art h2{font-size:32px;font-weight:700;margin:64px 0 18px;padding-top:24px;border-top:2px solid var(--pink);scroll-margin-top:90px}
.alg-art h3{font-size:22px;font-weight:700;margin:36px 0 10px}
.alg-art p{margin:0 0 16px}
.alg-art a{color:var(--brand);text-decoration:underline;text-underline-offset:3px}
.alg-art a:hover{color:var(--coral)}
.alg-art ul,.alg-art ol{margin:0 0 18px;padding-left:24px}
.alg-art li{margin-bottom:6px}
.alg-art ul li::marker{color:var(--brand)}
.alg-art ol li::marker{color:var(--brand);font-weight:700}
.alg-byline{font-size:15px;color:var(--grey);margin:0 0 24px;line-height:2}
.alg-byline span{background:var(--pink);color:var(--brand);border-radius:999px;padding:3px 12px;font-weight:600;margin-right:10px}
.alg-lead{font-size:20px;color:var(--ink)}
.alg-toc{background:#fff7f6;border:1px solid var(--line);border-radius:20px;padding:24px 28px;margin:28px 0 8px}
.alg-toc b{display:block;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-size:14px;letter-spacing:.08em;text-transform:uppercase;color:var(--brand);margin-bottom:12px}
.alg-toc ol{columns:2;column-gap:32px;margin:0;padding-left:22px}
.alg-toc a{text-decoration:none;color:var(--ink)}
.alg-toc a:hover{color:var(--brand)}
.alg-note{background:var(--pink);border-left:5px solid var(--brand);border-radius:14px;padding:18px 22px;margin:22px 0}
.alg-note p:last-child{margin:0}
.alg-promo{background:var(--brand);color:#fff;border-radius:20px;padding:26px 28px;margin:30px 0}
.alg-promo p{margin:0 0 14px}
.alg-promo a{color:#fff}
.alg-promo .alg-btn{background:#fff;color:var(--brand)!important}
.alg-btn{display:inline-block;background:var(--brand);color:#fff!important;text-decoration:none!important;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:600;font-size:16px;border-radius:12px;padding:13px 26px;transition:opacity .2s}
.alg-btn:hover{opacity:.88}
.alg-cards{display:grid;grid-template-columns:repeat(2,1fr);gap:14px;margin:18px 0 22px}
.alg-card{border:1px solid var(--line);border-radius:16px;padding:18px 20px;background:#fff;font-size:16px;line-height:1.55}
.alg-card a{display:block;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:700;font-size:17px;text-decoration:none;margin-bottom:6px;color:var(--ink)}
.alg-card a:hover{color:var(--brand)}
.alg-card a::after{content:" ↗";color:var(--brand);font-weight:400}
.alg-art .alg-steps{list-style:none;padding:0;counter-reset:s}
.alg-steps li{counter-increment:s;position:relative;padding:4px 0 10px 52px;margin:0}
.alg-steps li::before{content:counter(s);position:absolute;left:0;top:0;width:36px;height:36px;border-radius:50%;background:var(--brand);color:#fff;font-weight:700;display:flex;align-items:center;justify-content:center;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif}
.alg-table{width:100%;border-collapse:separate;border-spacing:0;margin:18px 0 24px;font-size:16px;border:1px solid var(--line);border-radius:14px;overflow:hidden}
.alg-table th{background:var(--brand);color:#fff;text-align:left;padding:12px 14px;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:600}
.alg-table td{padding:12px 14px;border-top:1px solid var(--line);vertical-align:top}
.alg-table tr:nth-child(even) td{background:#fff7f6}
.alg-faq details{border:1px solid var(--line);border-radius:14px;margin:0 0 10px;background:#fff}
.alg-faq summary{cursor:pointer;list-style:none;padding:16px 52px 16px 20px;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:600;font-size:17px;position:relative}
.alg-faq summary::-webkit-details-marker{display:none}
.alg-faq summary::after{content:"+";position:absolute;right:20px;top:50%;transform:translateY(-50%);font-size:26px;color:var(--brand);font-weight:400}
.alg-faq details[open] summary::after{content:"–"}
.alg-faq details p{padding:0 20px 16px;margin:0}
.alg-sources{font-size:15px;color:var(--grey)}
.alg-final{text-align:center;background:#fff7f6;border-radius:20px;padding:34px 24px;margin-top:48px}
.alg-final p{font-size:19px;margin-bottom:18px}
.alg-fig{margin:26px 0 30px}
.alg-fig img{display:block;width:100%;height:auto;aspect-ratio:16/9;object-fit:cover;border-radius:20px}
.alg-fig figcaption{font-size:14px;color:var(--grey);margin-top:10px;text-align:center}
.alg-duo{display:grid;grid-template-columns:1fr 1fr;gap:14px}
.alg-duo img{aspect-ratio:4/3}
.alg-duo figcaption{grid-column:1/-1;margin-top:0}
.alg-tl{display:flex;gap:0;margin:26px 0 30px;position:relative}
.alg-tl-item{flex:1;position:relative;padding:44px 10px 0;text-align:center;font-size:15px;line-height:1.45}
.alg-tl-item::before{content:"";position:absolute;top:15px;left:0;right:0;height:3px;background:var(--pink)}
.alg-tl-item:first-child::before{left:50%}.alg-tl-item:last-child::before{right:50%}
.alg-tl-item::after{content:"";position:absolute;top:6px;left:50%;transform:translateX(-50%);width:21px;height:21px;border-radius:50%;background:var(--brand);box-shadow:0 0 0 5px #fff}
.alg-tl-item b{display:block;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;color:var(--brand);font-size:16px;margin-bottom:4px}
.alg-ages{display:flex;align-items:flex-end;gap:12px;margin:24px 0 30px;height:300px}
.alg-age{flex:1;border-radius:16px 16px 6px 6px;background:var(--pink);padding:14px 12px;display:flex;flex-direction:column;justify-content:flex-start;font-size:14px;line-height:1.4}
.alg-age b{font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-size:17px;color:var(--brand);margin-bottom:4px}
.alg-age:nth-child(1){height:52%}.alg-age:nth-child(2){height:68%}.alg-age:nth-child(3){height:84%}
.alg-age:nth-child(4){height:100%;background:var(--brand);color:#fff}.alg-age:nth-child(4) b{color:#fff}
.alg-khda{display:grid;grid-template-columns:repeat(6,1fr);gap:6px;margin:20px 0 8px}
.alg-khda div{border-radius:10px;padding:14px 6px;text-align:center;color:#fff;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:600;font-size:14px;line-height:1.25}
.alg-khda-cap{display:flex;justify-content:space-between;font-size:13px;color:var(--grey);margin-bottom:26px}
@media (max-width:640px){
 .alg-art{font-size:16px;padding:0 16px 56px}
 .alg-lead{font-size:18px}
 .alg-art h2{font-size:25px;margin-top:48px}
 .alg-art h3{font-size:19px}
 .alg-toc{padding:20px}
 .alg-toc ol{columns:1}
 .alg-cards{grid-template-columns:1fr}
 .alg-table{font-size:14px}
 .alg-table th,.alg-table td{padding:10px}
 .alg-tl{flex-direction:column;gap:0}
 .alg-tl-item{text-align:left;padding:0 0 18px 40px}
 .alg-tl-item::before{top:0;bottom:0;left:10px;right:auto;width:3px;height:auto}
 .alg-tl-item:first-child::before{left:10px;top:12px}.alg-tl-item:last-child::before{right:auto;bottom:auto;height:12px}
 .alg-tl-item::after{top:2px;left:0;transform:none}
 .alg-ages{height:auto;flex-direction:column;align-items:stretch}
 .alg-age{height:auto!important;border-radius:14px}
 .alg-khda{grid-template-columns:repeat(3,1fr)}
 .alg-fig img{border-radius:14px}
 .alg-duo{gap:8px}
}
.alg-card b{display:block;font-family:var(--t-headline-font,'Montserrat'),Arial,sans-serif;font-weight:700;font-size:17px;color:var(--brand);margin-bottom:8px}
.alg-card ul{margin:0;padding-left:20px}
.alg-card li{margin-bottom:4px}
</style>

<article class="alg-art" lang="ru" itemscope itemtype="https://schema.org/Article">
<meta itemprop="headline" content="Подготовка к школе в Дубае: что должен уметь ребёнок в 5-6 лет">

<p class="alg-byline"><span>Гид для родителей</span> Команда образовательного центра «Алгоритм» · Обновлено <time datetime="2026-11-26">26 ноября 2026</time></p>

<p class="alg-lead">В Дубае вопрос «готов ли ребёнок к школе» сложнее, чем дома. Важно не только, умеет ли он читать и считать, но и на каком языке. Одни семьи готовятся к российскому первому классу, другие к Year 1 в британской школе, третьи хотят оставить открытыми оба варианта.</p>

<p>Разбираем, какие навыки действительно нужны к 6 годам и как их развивать, не превращая детство в бесконечные занятия.</p>

<figure class="alg-fig"><img src="https://algorithmdubai-production.up.railway.app/blog-images/kids-shapes-activity-with-parents.webp" alt="Дети раскладывают цветные фигуры на открытом занятии, родители наблюдают" width="960" height="540"><figcaption>Готовность к школе это не только чтение и счёт, но и умение работать в группе</figcaption></figure>

<nav class="alg-toc" aria-label="Содержание">
<b>Содержание</b>
<ol>
<li><a href="#when">Когда начинать</a></li>
<li><a href="#checklist">Чек-лист готовности</a></li>
<li><a href="#international">Если впереди международная школа</a></li>
<li><a href="#russian-school">Если впереди российская программа</a></li>
<li><a href="#home">7 привычек для дома</a></li>
<li><a href="#specialist">Когда нужен специалист</a></li>
<li><a href="#algorithm">Подготовка в «Алгоритме»</a></li>
<li><a href="#faq">Частые вопросы</a></li>
</ol>
</nav>

<h2 id="when">Когда начинать подготовку</h2>
<p>Лучше всего за год до школы, в 5-5,5 лет. Этого хватает, чтобы спокойно освоить грамоту и счёт, не торопя ребёнка.</p>
<p>Если ребёнок ходит в англоязычный детский сад, с русским стоит начать ещё раньше. К 5 годам у многих детей в Дубае английский становится основным языком игры и общения, а русский остаётся «домашним».</p>

<h2 id="checklist">Чек-лист: что должен уметь ребёнок к школе</h2>
<p>Это ориентир, а не экзамен. Если какого-то навыка пока нет, это повод уделить ему внимание, а не ставить диагноз.</p>

<div class="alg-cards">
<div class="alg-card"><b>Речь</b><ul><li>Пересказывает короткую сказку своими словами.</li><li>Составляет рассказ по картинке из 4-5 предложений.</li><li>Правильно произносит звуки родного языка.</li><li>Задаёт вопросы и объясняет, чего хочет.</li></ul></div>
<div class="alg-card"><b>Грамота и чтение</b><ul><li>Знает буквы, различает гласные и согласные, твёрдые и мягкие звуки.</li><li>Читает по слогам простые слова.</li><li>Пишет печатными буквами своё имя.</li></ul></div>
<div class="alg-card"><b>Математика</b><ul><li>Считает до 20 и обратно, знает состав чисел до 10.</li><li>Решает простые задачи «больше, меньше», «прибавить, отнять».</li><li>Различает фигуры, ориентируется на листе: вверху справа, под линией.</li></ul></div>
<div class="alg-card"><b>Мелкая моторика</b><ul><li>Правильно держит карандаш.</li><li>Обводит по контуру и штрихует, не выходя за линии.</li><li>Режет ножницами, лепит, собирает мелкий конструктор.</li></ul></div>
<div class="alg-card"><b>Внимание и поведение</b><ul><li>15-20 минут занимается одним делом.</li><li>Выполняет инструкцию из 2-3 шагов.</li><li>Доводит начатое до конца.</li><li>Спокойно переносит проигрыш в игре.</li></ul></div>
<div class="alg-card"><b>Самостоятельность</b><ul><li>Сам одевается, справляется с застёжками и обувью.</li><li>Собирает свой рюкзак, следит за вещами.</li><li>Может обратиться к взрослому за помощью.</li></ul></div>
</div>

<h2 id="international">Если ребёнок пойдёт в международную школу</h2>
<p>С 2026-27 учебного года в британских школах Дубая, где учёба начинается в сентябре, класс для новых учеников определяют по возрасту на 31 декабря: FS1 с 3 лет, FS2 с 4 лет, Year 1 с 5 лет.</p>
<p>На вступительном тестировании (assessment) обычно смотрят:</p>
<ul>
<li>понимает ли ребёнок английскую речь и простые инструкции;</li>
<li>знает ли буквы и звуки английского, чаще всего по методике phonics;</li>
<li>как считает и знает ли базовые математические понятия;</li>
<li>умеет ли общаться и работать в группе.</li>
</ul>
<p>Самая частая сложность у русскоязычных детей связана с языком, а не со знаниями: ребёнок умеет решить задачу, но не понимает, что от него хотят. Поэтому подготовка к международной школе это прежде всего английский в учебных ситуациях: слушать учителя, отвечать на вопросы, работать с заданиями.</p>
<p>О выборе школы и поступлении подробно рассказываем в статье <a href="/kak-vybrat-shkolu-v-dubae">«Как выбрать школу в Дубае»</a>.</p>

<h2 id="russian-school">Если ребёнок пойдёт на российскую программу</h2>
<p>В российском первом классе нужно читать и писать по-русски, а для ребёнка, который живёт в англоязычной среде, это отдельная задача. Дети, которые свободно говорят по-русски дома, часто удивляют родителей на диагностике: устная речь хорошая, а звуковой анализ слов, чтение и письмо отстают от сверстников в России.</p>
<p>Здесь важна регулярность. Два-три занятия в неделю с педагогом дают больше, чем интенсивная подготовка за месяц до школы.</p>

<figure class="alg-fig"><img src="https://algorithmdubai-production.up.railway.app/blog-images/shkola-rossii-workbooks.webp" alt="Рабочие тетради «Школа России» для 1 класса: русский язык, математика, окружающий мир" width="960" height="540" loading="lazy"><figcaption>Для российского первого класса ребёнку нужно читать и писать по-русски</figcaption></figure>

<h2 id="home">Как готовить ребёнка дома: 7 простых привычек</h2>
<ol class="alg-steps">
<li><b>Читайте вслух каждый день</b> на том языке, который сложнее удерживать. Обсуждайте прочитанное: «Почему герой так поступил?»</li>
<li><b>Играйте в слова:</b> «назови слово на звук М», «какой звук последний в слове кот».</li>
<li><b>Считайте в быту:</b> тарелки на столе, ступеньки, монеты, машины на парковке.</li>
<li><b>Давайте поручения из нескольких шагов:</b> «возьми книгу, положи на стол и позови папу».</li>
<li><b>Рисуйте, лепите, вырезайте.</b> Это лучшая подготовка руки к письму.</li>
<li><b>Учите доводить дело до конца:</b> собранный пазл, дорисованная картинка, убранные игрушки.</li>
<li><b>Не сравнивайте</b> ребёнка с другими детьми. У билингвов один из языков почти всегда развивается быстрее, и это нормально.</li>
</ol>

<h2 id="specialist">Когда нужна помощь специалиста</h2>
<p>Стоит показать ребёнка педагогу или логопеду, если:</p>
<ul>
<li>к 5 годам заметно нарушено звукопроизношение;</li>
<li>ребёнку трудно удерживать внимание даже на интересном занятии;</li>
<li>он избегает рисования и любых заданий с карандашом;</li>
<li>путает языки так, что его не понимают ни на одном из них.</li>
</ul>

<div class="alg-promo">
<p>Начните с бесплатной диагностики в «Алгоритме»: педагог оценит готовность к школе и уровень русского языка и подскажет, какой формат подготовки подойдёт.</p>
<a class="alg-btn" href="/dia">Записаться на диагностику</a>
</div>

<h2 id="algorithm">Подготовка к школе в «Алгоритме»</h2>
<p>В центре есть два формата <a href="/preparatory">подготовки к школе для детей от 5,5 лет</a>:</p>
<table class="alg-table">
<thead><tr><th>Формат</th><th>Когда</th><th>Что внутри</th></tr></thead>
<tbody>
<tr><td><b>По субботам</b></td><td>Суббота, 09:00-13:00</td><td>Грамота и письмо на русском, математика, окружающий мир, развитие речи. Подходит, если ребёнок ходит в англоязычный сад, а русский важно поддерживать без перегрузки в будни.</td></tr>
<tr><td><b>Пять дней в неделю</b></td><td>Понедельник-пятница, 09:00-13:00</td><td>Комплексная подготовка, в том числе к международной школе: русский язык, математика, окружающий мир, развитие речи и чтения плюс усиленный английский (Jolly Phonics, First Math, Storytelling).</td></tr>
</tbody>
</table>
<p>Программы составлены с учётом ФГОС.</p>

<h2 id="faq">Частые вопросы</h2>
<div class="alg-faq">
<details><summary>Во сколько лет начинать подготовку к школе?</summary><p>Лучше всего за год до школы, в 5-5,5 лет. Если ребёнок ходит в англоязычный сад, русский стоит поддерживать раньше.</p></details>
<details><summary>Нужно ли учить ребёнка читать до школы?</summary><p>Для российского первого класса желательно читать по слогам. В британской системе чтению учат в FS2 и Year 1 через phonics, но знание букв и звуков даст ребёнку уверенность на старте.</p></details>
<details><summary>Как понять, готов ли ребёнок к школе?</summary><p>Ориентируйтесь на чек-лист: речь, грамота, счёт, моторика, внимание и самостоятельность. Объективную оценку даст диагностика у педагога.</p></details>
<details><summary>Можно ли готовиться сразу к российской и международной школе?</summary><p>Да, если правильно распределить нагрузку: основные предметы на русском и регулярная практика английского. Так устроена пятидневная подготовка в «Алгоритме».</p></details>
<details><summary>С какого возраста берут в Year 1 в Дубае?</summary><p>С 2026-27 учебного года в школах с началом учёбы в сентябре в Year 1 принимают детей, которым до 31 декабря исполняется 5 лет.</p></details>
</div>

<h2 id="sources">Источники</h2>
<div class="alg-sources">
<ul>
<li><a href="https://www.khaleejtimes.com/uae/dubai-school-admissions-khda-new-guide-age-cut-off?utm_source=algorithmdubai&utm_medium=referral&utm_campaign=blog_preparatory" target="_blank" rel="noopener">Khaleej Times</a>: новые возрастные правила приёма в школы Дубая с 2026-27 учебного года.</li>
</ul>
</div>

<div class="alg-final">
<p>Узнайте, готов ли ребёнок к школе, на бесплатной диагностике, а все форматы подготовки смотрите на странице программы.</p>
<a class="alg-btn" href="/preparatory">Подготовка к школе</a>
</div>
</article>

<script type="application/ld+json">
{
 "@context": "https://schema.org",
 "@graph": [
  {
   "@type": "Article",
   "headline": "Подготовка к школе в Дубае: что должен уметь ребёнок в 5-6 лет",
   "description": "Чек-лист готовности к школе для детей 5-6 лет: речь, чтение, счёт, английский, внимание и самостоятельность. Как готовить ребёнка к российской и международной школе.",
   "inLanguage": "ru",
   "datePublished": "2026-11-26",
   "dateModified": "2026-11-26",
   "mainEntityOfPage": "https://algorithmdubai.com/podgotovka-k-shkole-v-dubae",
   "image": "https://algorithmdubai-production.up.railway.app/blog-images/kids-shapes-activity-with-parents.webp",
   "author": {
    "@type": "Organization",
    "name": "Образовательный центр «Алгоритм»",
    "url": "https://algorithmdubai.com/ru"
   },
   "publisher": {
    "@type": "Organization",
    "name": "Образовательный центр «Алгоритм»",
    "url": "https://algorithmdubai.com/ru"
   }
  },
  {
   "@type": "BreadcrumbList",
   "itemListElement": [
    {
     "@type": "ListItem",
     "position": 1,
     "name": "Главная",
     "item": "https://algorithmdubai.com/ru"
    },
    {
     "@type": "ListItem",
     "position": 2,
     "name": "Блог",
     "item": "https://algorithmdubai.com/blog-ru"
    },
    {
     "@type": "ListItem",
     "position": 3,
     "name": "Подготовка к школе в Дубае",
     "item": "https://algorithmdubai.com/podgotovka-k-shkole-v-dubae"
    }
   ]
  },
  {
   "@type": "FAQPage",
   "mainEntity": [
    {
     "@type": "Question",
     "name": "Во сколько лет начинать подготовку к школе?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Лучше всего за год до школы, в 5-5,5 лет. Если ребёнок ходит в англоязычный сад, русский стоит поддерживать раньше."
     }
    },
    {
     "@type": "Question",
     "name": "Нужно ли учить ребёнка читать до школы?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Для российского первого класса желательно читать по слогам. В британской системе чтению учат в FS2 и Year 1 через phonics, но знание букв и звуков даст ребёнку уверенность на старте."
     }
    },
    {
     "@type": "Question",
     "name": "Как понять, готов ли ребёнок к школе?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Ориентируйтесь на чек-лист: речь, грамота, счёт, моторика, внимание и самостоятельность. Объективную оценку даст диагностика у педагога."
     }
    },
    {
     "@type": "Question",
     "name": "Можно ли готовиться сразу к российской и международной школе?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Да, если правильно распределить нагрузку: основные предметы на русском и регулярная практика английского. Так устроена пятидневная подготовка в «Алгоритме»."
     }
    },
    {
     "@type": "Question",
     "name": "С какого возраста берут в Year 1 в Дубае?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "С 2026-27 учебного года в школах с началом учёбы в сентябре в Year 1 принимают детей, которым до 31 декабря исполняется 5 лет."
     }
    }
   ]
  }
 ]
}
</script>
```

---

## Отчёт, который нужно вернуть

Для каждой статьи: опубликованный адрес, что сделано по шагам 1-11, что не получилось и почему (со скриншотом), значения formname во всех трёх формах.
