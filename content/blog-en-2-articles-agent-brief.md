# Задача для браузерного агента: сверстать английские версии 2 статей блога «Алгоритм Дубай» в Тильде

## Кто ты и что делаешь

Ты работаешь в Тильде в проекте сайта **algorithmdubai.com** (образовательный центр Algorithm Training Center в Дубае). Нужно опубликовать английские версии двух статей, русские версии которых уже опубликованы:

- https://algorithmdubai.com/kak-vybrat-shkolu-v-dubae
- https://algorithmdubai.com/podgotovka-k-shkole-v-dubae

Перевод, вёрстка, SEO-настройки и разметка готовы: ниже полный HTML-код каждой статьи. Твоя работа: создать страницы, вставить код, заполнить настройки, задать названия форм для CRM, добавить hreflang, опубликовать, добавить карточки в английский блог и проверить.

**Порядок важен:** сначала статья 1 (How to Choose a School), потом статья 2 (Preparing for School), потому что статья 2 ссылается на статью 1.

## Как устроен английский блог сейчас

- Опубликованная статья-образец: **https://algorithmdubai.com/living-in-dubai-with-kids** («Living in Dubai with Kids»). Структура страницы сверху вниз:
  1. английское меню с переключателем RU;
  2. блок с заголовком статьи и подписью;
  3. блок **T123 «HTML-код»** с самой статьёй (стили, текст, картинки, FAQ, разметка schema.org и скрипт переключателя языка уже внутри кода);
  4. попап `#reg`, попап пробного урока и красная форма консультации (всё на английском);
  5. FAQ центра, контакты, подвал на английском.
- Хаб английского блога: **https://algorithmdubai.com/blog**, на нём карточка гида с кнопкой чтения.

## Пошагово для каждой статьи

1. В проекте Тильды найди страницу **living-in-dubai-with-kids** и сделай её **копию** (Дублировать страницу). Работай только с копией, оригинал не меняй.
2. Открой копию. В блоке с заголовком статьи замени текст на H1 из карточки статьи ниже. Назначь этому тексту тег **H1** (Zero-блок: элемент → настройки → SEO → тег H1; обычный блок: настройки блока → тег заголовка H1). Других H1 на странице быть не должно. Это обязательный шаг: у текущих статей блога H1 нет, и это главная SEO-ошибка, которую мы исправляем.
3. Найди блок **T123 «HTML-код»** со статьёй-гидом. Открой «Контент» блока, **полностью удали** старый код и вставь код статьи из раздела ниже целиком, от первой строки `<!--` до последней `</script>`. Сохрани.
4. **Настройки страницы → Главное:** заголовок (title), описание (description) и адрес страницы из карточки статьи (латиница, без слеша в начале).
5. **Настройки страницы → Соцсети:** заголовок и описание из карточки. Картинка: скачай по ссылке «Картинка для соцсетей» и загрузи.
6. **Настройки страницы → SEO/индексация:** запрет индексации снят.
7. **Настройки страницы → Дополнительно → HTML-код для вставки внутрь HEAD:** вставь код hreflang из карточки статьи. Если в поле уже есть код, скопированный с гида, удали из него старые строки `hreflang` и canonical, остальное не трогай.
8. **Формы для CRM.** На странице есть попап `#reg`, попап пробного урока и красная форма консультации. В каждой форме открой «Контент» → поля → скрытые поля (hidden) и задай значения из карточки:
   - скрытое поле `formname` и одноимённое название формы;
   - скрытое поле `programs`: такое же значение, как formname.

   Получатели данных (интеграции с CRM) **не трогай**. Если какое-то скрытое поле не находится, не создавай новое: скрипт в конце кода статьи подставит правильные названия сам. Просто отметь это в отчёте.
9. Блоки ниже статьи (FAQ центра, контакты, подвал) оставь как в гиде.
10. Нажми **Опубликовать**.
11. На странице **blog** продублируй карточку гида и замени картинку, заголовок, текст и ссылку кнопки на данные из карточки статьи. Опубликуй blog.

## После обеих статей: hreflang на русских версиях

Открой страницы **kak-vybrat-shkolu-v-dubae** и **podgotovka-k-shkole-v-dubae** → Настройки страницы → Дополнительно → HTML-код для вставки внутрь HEAD. Добавь в конец поля код из блока «HEAD для русской версии» в карточке соответствующей статьи (существующий код не удаляй). Опубликуй обе страницы.

Этот же код переключает кнопку языка «En» в меню русской статьи на её английскую версию.

## Чего не делать

- Не менять оригинальную страницу living-in-dubai-with-kids и другие страницы сайта, кроме blog и двух русских статей (только поле HEAD).
- Не редактировать текст внутри HTML-кода статьи: он вычитан и проверен.
- Не менять получателей данных у форм и настройки проекта.
- Не добавлять второй H1.
- Тестовую заявку **не отправлять**.

## Проверка после публикации

- Адрес открывается, H1 правильный и один.
- В статье видны картинки, таблица, оглавление, раскрывающиеся вопросы FAQ.
- Кнопки «Book a free assessment» и «Book a consultation» открывают попап записи.
- Кнопка «RU» в меню ведёт на русскую версию этой статьи, а «En» на русской статье ведёт на английскую.
- В статье 2 ссылка «How to Choose a School in Dubai» открывает статью 1.
- В исходном коде (view-source) есть title и description из карточки и строки `hreflang="ru"` и `hreflang="en"`.
- Карточки обеих статей видны на https://algorithmdubai.com/blog и ведут на правильные адреса.

---

## Статья 1. How to Choose a School in Dubai

| Поле | Значение |
|---|---|
| Название страницы в Тильде | Blog EN: How to Choose a School in Dubai |
| Адрес страницы | `how-to-choose-a-school-in-dubai` |
| H1 (заголовок в блоке над статьёй) | How to Choose a School in Dubai: Curricula, KHDA Ratings and Admissions |
| Title (60 симв.) | `How to Choose a School in Dubai: Curricula, KHDA, Admissions` |
| Description | `British, American or IB? How to read KHDA ratings, which documents you need, how much the deposit is and how to prepare your child for a Dubai school.` |
| Соцсети: заголовок | How to Choose a School in Dubai: a Step-by-Step Plan for Parents |
| Соцсети: описание | Curricula, KHDA ratings, documents, deposits and the entrance assessment. A guide from Algorithm Training Center. |
| Картинка для соцсетей | https://algorithmdubai-production.up.railway.app/blog-images/classroom-pupils-at-desks.webp |
| formname и programs, попап #reg | `Blog eng school: program selection` |
| formname и programs, попап пробного урока | `Blog eng school: lesson` |
| formname и programs, красная форма | `Blog eng school: consultation and dia` |
| Карточка на /blog: заголовок | How to Choose a School in Dubai |
| Карточка на /blog: текст | British, American or IB, KHDA ratings, documents and admissions |
| Карточка на /blog: картинка | https://algorithmdubai-production.up.railway.app/blog-images/classroom-pupils-at-desks.webp |
| Карточка на /blog: ссылка | `https://algorithmdubai.com/how-to-choose-a-school-in-dubai` |
| Русская версия | https://algorithmdubai.com/kak-vybrat-shkolu-v-dubae |

### HEAD для английской страницы /how-to-choose-a-school-in-dubai

```html
<link rel="canonical" href="https://algorithmdubai.com/how-to-choose-a-school-in-dubai">
<link rel="alternate" hreflang="en" href="https://algorithmdubai.com/how-to-choose-a-school-in-dubai">
<link rel="alternate" hreflang="ru" href="https://algorithmdubai.com/kak-vybrat-shkolu-v-dubae">
<link rel="alternate" hreflang="x-default" href="https://algorithmdubai.com/how-to-choose-a-school-in-dubai">
<meta property="og:locale" content="en_US">
```

### HEAD для русской версии /kak-vybrat-shkolu-v-dubae (добавить в конец поля)

```html
<link rel="alternate" hreflang="ru" href="https://algorithmdubai.com/kak-vybrat-shkolu-v-dubae">
<link rel="alternate" hreflang="en" href="https://algorithmdubai.com/how-to-choose-a-school-in-dubai">
<link rel="alternate" hreflang="x-default" href="https://algorithmdubai.com/how-to-choose-a-school-in-dubai">
<script>
document.addEventListener('DOMContentLoaded',function(){document.querySelectorAll('a').forEach(function(a){if(a.textContent.trim().toLowerCase()==='en')a.setAttribute('href','https://algorithmdubai.com/how-to-choose-a-school-in-dubai');});});
</script>
```

### HTML-код статьи 1 (вставить целиком в блок T123)

```html
<!-- Algorithm Dubai · How to Choose a School in Dubai (EN) · paste into the T123 HTML block on /how-to-choose-a-school-in-dubai -->
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

<article class="alg-art" lang="en" itemscope itemtype="https://schema.org/Article">
<meta itemprop="headline" content="How to Choose a School in Dubai: Curricula, KHDA Ratings and Admissions">

<p class="alg-byline"><span>Parent's guide</span> By the Algorithm Training Center team · Updated <time datetime="2026-11-26">26 November 2026</time></p>

<p class="alg-lead">Your choice of school in Dubai shapes a lot: which language your child will think in a couple of years from now, which universities they can apply to and who their friends will be. And the choice is huge: the emirate has hundreds of private schools teaching a dozen different curricula.</p>

<p>Here's the step-by-step approach that helps families at our centre narrow the list down to two or three schools and get through admissions calmly.</p>

<figure class="alg-fig"><img src="https://algorithmdubai-production.up.railway.app/blog-images/classroom-pupils-at-desks.webp" alt="Pupils listening to the teacher at their desks in a bright classroom" width="960" height="540"><figcaption>Choose the curriculum first, then the school</figcaption></figure>

<nav class="alg-toc" aria-label="Contents">
<b>Contents</b>
<ol>
<li><a href="#program">Choose a curriculum</a></li>
<li><a href="#khda">Check the KHDA rating</a></li>
<li><a href="#practical">Commute and costs</a></li>
<li><a href="#tour">Book a school tour</a></li>
<li><a href="#documents">Prepare the documents</a></li>
<li><a href="#assessment">Take the assessment</a></li>
<li><a href="#prepare">How to prepare your child</a></li>
<li><a href="#russian">Keeping Russian alive</a></li>
<li><a href="#faq">FAQ</a></li>
</ol>
</nav>

<h2 id="program">Step 1. Decide which curriculum suits your child</h2>
<p>The curriculum matters more than the school's name. It decides the exams, the workload and which universities will be easier to apply to later.</p>

<table class="alg-table">
<thead><tr><th>Curriculum</th><th>Final exams</th><th>Best for</th></tr></thead>
<tbody>
<tr><td><b>British</b></td><td>IGCSE at 16, A-Levels at 18</td><td>Families looking at universities in the UK and Europe who like a clear, exam-based system</td></tr>
<tr><td><b>American</b></td><td>High School Diploma and GPA, plus SAT or ACT for US universities</td><td>Families planning on the US or Canada, and children who work steadily through the year</td></tr>
<tr><td><b>IB</b></td><td>IB Diploma after the last two years (DP)</td><td>Independent learners: lots of projects, essays and research, recognised by universities worldwide</td></tr>
</tbody>
</table>

<h3>British curriculum</h3>
<p>The most common curriculum in Dubai. Learning is split into Key Stages. Students take IGCSEs at 16 and A-Levels at 18, and these exams are accepted by British and many other universities.</p>

<h3>American curriculum</h3>
<p>A wide choice of subjects and a cumulative grading system (GPA), ending with a High School Diploma. Students applying to US universities also take the SAT or ACT.</p>

<h3>IB programme</h3>
<p>The International Baccalaureate has three stages: PYP in primary, MYP in middle school and DP in the last two years. The IB Diploma is recognised by universities around the world. It's considered one of the most demanding programmes, with a lot of research projects, essays and independent work.</p>

<h3>Other options</h3>
<p>Dubai also has schools with Indian (CBSE, ICSE), French, German and other national curricula. There are very few schools offering the full Russian curriculum, so Russian-speaking families usually choose an international school and keep up the Russian programme alongside it.</p>

<h2 id="khda">Step 2. Check the school's KHDA rating</h2>
<p>Private schools in Dubai are regulated by the KHDA (Knowledge and Human Development Authority). After an inspection, each school gets an overall rating on a six-point scale:</p>

<div class="alg-khda" role="list" aria-label="KHDA school rating scale">
<div role="listitem" style="background:#1f7a4d">Outstanding</div><div role="listitem" style="background:#4c9a5a">Very Good</div><div role="listitem" style="background:#8bb54a">Good</div><div role="listitem" style="background:#d9a52b">Acceptable</div><div role="listitem" style="background:#e1625c">Weak</div><div role="listitem" style="background:#9e2744">Very Weak</div>
</div>
<div class="alg-khda-cap"><span>Highest rating</span><span>Lowest rating</span></div>

<p>Inspectors look at attainment and progress, quality of teaching, safety, support for children with special needs, and Arabic and Islamic studies.</p>

<div class="alg-note">
<p>The KHDA didn't run regular inspections of most schools in 2024-25 and 2025-26, so most schools still carry the rating from their last inspection. Alongside the overall rating, each school's page in the KHDA directory has a short parent summary report on teaching quality and student wellbeing.</p>
</div>

<p>How to use the ratings:</p>
<ul>
<li><b>Read the report, not just the overall rating.</b> A school can be Outstanding for English and Good for maths.</li>
<li><b>Look at the trend.</b> A school that has moved up from Good to Very Good can be more interesting than one that has held the same rating for years.</li>
<li><b>A rating doesn't replace a visit.</b> It won't show you the atmosphere, how teachers treat children or how the school supports pupils for whom English is a second language.</li>
</ul>
<p>Ratings and reports are published on the KHDA website and app.</p>

<h2 id="practical">Step 3. Think about the commute and costs</h2>
<p><b>Commute.</b> Dubai is big, and a school 40 minutes away means almost an hour and a half in the car every day. Ask whether the school bus serves your area.</p>
<p><b>Costs.</b> Fees vary a lot from school to school and go up with each year group. On top of tuition fees, budget for the application fee, the seat deposit, uniform, transport, meals and clubs. Schools publish their current fees on their websites.</p>
<p><b>English support.</b> If your child has just arrived, ask about EAL (English as an Additional Language): how it works, how many hours a week it runs and when children move into mainstream classes.</p>
<p><b>Other Russian speakers in the class.</b> They make the first months easier. But if there are too many, English may develop more slowly.</p>

<h2 id="tour">Step 4. Book a school tour</h2>
<p>Pick three to five schools and book a school tour. Questions worth asking:</p>
<ul>
<li>How many children are in a class, and how many teaching assistants?</li>
<li>How does the school support children who don't speak much English yet?</li>
<li>How often do parents get feedback?</li>
<li>Which clubs are included in the fees, and which cost extra?</li>
<li>Are there places in the year group you need, and is there a waiting list?</li>
</ul>
<p>Watch how teachers talk to children in the corridors. It tells you more than any admissions presentation.</p>

<figure class="alg-fig"><img src="https://algorithmdubai-production.up.railway.app/blog-images/russian-class-girl-at-desk.webp" alt="Girl smiling at her desk during a lesson" width="960" height="540" loading="lazy"><figcaption>On a tour, watch how teachers talk to children</figcaption></figure>

<h2 id="documents">Step 5. Prepare the documents</h2>
<p>Each school has its own list, but you'll usually need:</p>
<ul>
<li>an online application and the application fee;</li>
<li>the child's and parents' passports;</li>
<li>residence visa and Emirates ID: you can apply without them, but they're required before your child starts;</li>
<li>birth certificate;</li>
<li>photos;</li>
<li>school reports from the last one or two years;</li>
<li>vaccination record;</li>
<li>a Transfer Certificate from the previous school.</li>
</ul>
<div class="alg-note">
<p>A Transfer Certificate is required for children joining Year 3 (Grade 2) and above from a school outside Dubai. If it was issued abroad, it has to be attested in the country of issue and by the UAE embassy. Your child can't start classes without it, so check the exact process with your chosen school early.</p>
</div>
<p>Documents in Russian usually need to be translated into English or Arabic.</p>

<h2 id="assessment">Step 6. Take the entrance assessment</h2>
<ol class="alg-steps">
<li>You submit the application and pay the application fee. Under KHDA rules it can't exceed AED 500 and isn't deducted from tuition.</li>
<li>Your child takes the assessment: English and maths, sometimes an interview. For younger children it's a play-based session, for older ones a written test.</li>
<li>If all goes well, the school sends an offer.</li>
<li>To secure the place, you pay a seat deposit. The KHDA caps it at 10% of the annual tuition fee, and it's then deducted from the fees.</li>
</ol>
<p>Many schools admit children throughout the year if there are places. Popular schools, though, have waiting lists a year or more ahead, so start early.</p>

<h3>Age at entry</h3>
<p>From the 2026-27 academic year, children registering at a Dubai school for the first time are placed by their age on 31 December. In schools that start in September, that means FS1 from age 3, FS2 from 4, Year 1 from 5 and Year 2 from 6.</p>

<h2 id="prepare">How to prepare your child for admission</h2>
<p>Russian-speaking children rarely struggle with the maths. They struggle with English: they don't understand how a task is worded, or get lost in an unfamiliar test format.</p>
<p>What helps:</p>
<ol>
<li><b>Check their level early,</b> six months before applying, not one month.</li>
<li><b>Practise the test format</b>, not just the language: picture-based tasks, logic puzzles, reading short texts against the clock.</li>
<li><b>Keep maths strong.</b> The Russian curriculum usually gives a solid foundation, and that's a real advantage in the test.</li>
</ol>

<div class="alg-promo">
<p>Not sure where your child's English and Russian are right now? Book a free assessment at Algorithm: a teacher will check their level and suggest where to start.</p>
<a class="alg-btn" href="#reg">Book a free assessment</a>
</div>

<h2 id="russian">How to keep your child's Russian alive</h2>
<p>An international school almost always crowds out Russian. After a year or two children still speak it, but reading and writing become hard. If you want to keep the language, or keep the option of going back to a Russian school, the Russian programme needs to run alongside international school.</p>
<p>At Algorithm we offer the Russian curriculum for international school students in Years 1-8, with classes on Fridays or Saturdays and online lessons during the week, and assessments taken in Dubai. We also run a five-day Russian programme for Years 1-4. <a href="https://algorithmdubai.com/#programs">See all programmes</a>.</p>

<h2 id="faq">FAQ</h2>
<div class="alg-faq">
<details><summary>How much does school cost in Dubai?</summary><p>It depends on the school, curriculum and year group, and fees can differ several times over. Check fees on school websites and budget for extras: application fee, seat deposit, uniform and transport.</p></details>
<details><summary>When should we apply to a school in Dubai?</summary><p>For popular schools, a year or more ahead. Many schools also admit children during the year if there are places, but the choice is smaller.</p></details>
<details><summary>What is a good KHDA rating?</summary><p>Outstanding and Very Good are the top levels, Good is solidly average. Read the full report: the overall rating doesn't show strengths and weaknesses by subject.</p></details>
<details><summary>Is there a Russian school in Dubai?</summary><p>There are very few schools with the full Russian curriculum in Dubai. Many families choose an international school and follow the Russian programme alongside it, for example in a hybrid format with assessments in Dubai.</p></details>
<details><summary>Does my child need English to get into a Dubai school?</summary><p>Yes, almost every school tests English. If your child's level is still low, look for schools with EAL support and start preparing early.</p></details>
<details><summary>How much is the deposit when a school offers a place?</summary><p>Under KHDA rules the application fee is up to AED 500 and the seat deposit is up to 10% of the annual tuition fee. The deposit is then deducted from the fees.</p></details>
</div>

<h2 id="sources">Sources</h2>
<div class="alg-sources">
<p>UAE rules change, so check official sources before you apply:</p>
<ul>
<li><a href="https://web.khda.gov.ae/en/Guides/Parents/A-Parent%E2%80%99s-Guide-to-Fees,-Deposits-and-Refunds-(1)?utm_source=algorithmdubai&utm_medium=referral&utm_campaign=blog_school_en" target="_blank" rel="noopener">KHDA</a>: fees, deposits and refunds at Dubai private schools;</li>
<li><a href="https://web.khda.gov.ae/en/About-Us/News/2025/KHDA-announces-pause-on-school-inspections-for-202?utm_source=algorithmdubai&utm_medium=referral&utm_campaign=blog_school_en" target="_blank" rel="noopener">KHDA</a>: pause on school inspections;</li>
<li><a href="https://www.khaleejtimes.com/uae/dubai-school-admissions-khda-new-guide-age-cut-off?utm_source=algorithmdubai&utm_medium=referral&utm_campaign=blog_school_en" target="_blank" rel="noopener">Khaleej Times</a>: new admission age rules from 2026-27.</li>
</ul>
</div>

<div class="alg-final">
<p>Algorithm Training Center in Dubai: school preparation, the Russian curriculum for international school students, and Russian and English courses for children.</p>
<a class="alg-btn" href="#reg">Book a consultation</a>
</div>
</article>

<script type="application/ld+json">
{
 "@context": "https://schema.org",
 "@graph": [
  {
   "@type": "Article",
   "headline": "How to Choose a School in Dubai: Curricula, KHDA Ratings and Admissions",
   "description": "British, American or IB? How to read KHDA ratings, which documents you need, how much the deposit is and how to prepare your child for a Dubai school.",
   "inLanguage": "en",
   "datePublished": "2026-11-26",
   "dateModified": "2026-11-26",
   "mainEntityOfPage": "https://algorithmdubai.com/how-to-choose-a-school-in-dubai",
   "image": "https://algorithmdubai-production.up.railway.app/blog-images/classroom-pupils-at-desks.webp",
   "author": {
    "@type": "Organization",
    "name": "Algorithm Training Center",
    "url": "https://algorithmdubai.com/"
   },
   "publisher": {
    "@type": "Organization",
    "name": "Algorithm Training Center",
    "url": "https://algorithmdubai.com/"
   }
  },
  {
   "@type": "BreadcrumbList",
   "itemListElement": [
    {
     "@type": "ListItem",
     "position": 1,
     "name": "Home",
     "item": "https://algorithmdubai.com/"
    },
    {
     "@type": "ListItem",
     "position": 2,
     "name": "Blog",
     "item": "https://algorithmdubai.com/blog"
    },
    {
     "@type": "ListItem",
     "position": 3,
     "name": "How to Choose a School in Dubai",
     "item": "https://algorithmdubai.com/how-to-choose-a-school-in-dubai"
    }
   ]
  },
  {
   "@type": "FAQPage",
   "mainEntity": [
    {
     "@type": "Question",
     "name": "How much does school cost in Dubai?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "It depends on the school, curriculum and year group, and fees can differ several times over. Check fees on school websites and budget for extras: application fee, seat deposit, uniform and transport."
     }
    },
    {
     "@type": "Question",
     "name": "When should we apply to a school in Dubai?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "For popular schools, a year or more ahead. Many schools also admit children during the year if there are places, but the choice is smaller."
     }
    },
    {
     "@type": "Question",
     "name": "What is a good KHDA rating?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Outstanding and Very Good are the top levels, Good is solidly average. Read the full report: the overall rating doesn't show strengths and weaknesses by subject."
     }
    },
    {
     "@type": "Question",
     "name": "Is there a Russian school in Dubai?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "There are very few schools with the full Russian curriculum in Dubai. Many families choose an international school and follow the Russian programme alongside it, for example in a hybrid format with assessments in Dubai."
     }
    },
    {
     "@type": "Question",
     "name": "Does my child need English to get into a Dubai school?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Yes, almost every school tests English. If your child's level is still low, look for schools with EAL support and start preparing early."
     }
    },
    {
     "@type": "Question",
     "name": "How much is the deposit when a school offers a place?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Under KHDA rules the application fee is up to AED 500 and the seat deposit is up to 10% of the annual tuition fee. The deposit is then deducted from the fees."
     }
    }
   ]
  }
 ]
}
</script>
<script>
(function(){
  var LANG={label:'RU',href:'https://algorithmdubai.com/kak-vybrat-shkolu-v-dubae'};
  var FORMS={"Blog eng: program selection": "Blog eng school: program selection", "Living in Dubai with kids: program selection": "Blog eng school: program selection", "Blog eng: lesson": "Blog eng school: lesson", "Living in Dubai with kids: lesson": "Blog eng school: lesson", "Blog eng: consultation and dia": "Blog eng school: consultation and dia", "Living in Dubai with kids: consultation and dia": "Blog eng school: consultation and dia"};
  function fix(){
    document.querySelectorAll('a').forEach(function(a){
      if(a.textContent.trim().toLowerCase()===LANG.label.toLowerCase()){a.setAttribute('href',LANG.href);}
    });
    document.querySelectorAll('input[name="formname"]').forEach(function(cur){
      var f=cur.form; if(!f) return;
      var key=cur.getAttribute('data-alg-orig')||cur.value; var m=FORMS[key]; if(!m) return;
      f.querySelectorAll('input[name="formname"],input[name="tildaspec-formname"],input[name="programs"]').forEach(function(x){x.setAttribute('data-alg-orig',key);x.value=m;});
    });
  }
  if(document.readyState!=='loading'){fix();}else{document.addEventListener('DOMContentLoaded',fix);}
  window.addEventListener('load',fix);
})();
</script>
```

## Статья 2. Preparing for School in Dubai

| Поле | Значение |
|---|---|
| Название страницы в Тильде | Blog EN: Preparing for School in Dubai |
| Адрес страницы | `preparing-for-school-in-dubai` |
| H1 (заголовок в блоке над статьёй) | Preparing for School in Dubai: What Your Child Should Know at 5-6 |
| Title (52 симв.) | `Preparing for School in Dubai: What Kids Need at 5-6` |
| Description | `A school readiness checklist for children aged 5-6: speech, reading, maths, English, attention and independence. How to prepare for Russian and international schools.` |
| Соцсети: заголовок | Is Your Child Ready for School? A Checklist for Parents in Dubai |
| Соцсети: описание | Speech, reading, maths, English and independence. How to prepare for Russian and international schools. |
| Картинка для соцсетей | https://algorithmdubai-production.up.railway.app/blog-images/kids-shapes-activity-with-parents.webp |
| formname и programs, попап #reg | `Blog eng prep: program selection` |
| formname и programs, попап пробного урока | `Blog eng prep: lesson` |
| formname и programs, красная форма | `Blog eng prep: consultation and dia` |
| Карточка на /blog: заголовок | Preparing for School in Dubai |
| Карточка на /blog: текст | A school readiness checklist for ages 5-6 and simple habits for home |
| Карточка на /blog: картинка | https://algorithmdubai-production.up.railway.app/blog-images/kids-shapes-activity-with-parents.webp |
| Карточка на /blog: ссылка | `https://algorithmdubai.com/preparing-for-school-in-dubai` |
| Русская версия | https://algorithmdubai.com/podgotovka-k-shkole-v-dubae |

### HEAD для английской страницы /preparing-for-school-in-dubai

```html
<link rel="canonical" href="https://algorithmdubai.com/preparing-for-school-in-dubai">
<link rel="alternate" hreflang="en" href="https://algorithmdubai.com/preparing-for-school-in-dubai">
<link rel="alternate" hreflang="ru" href="https://algorithmdubai.com/podgotovka-k-shkole-v-dubae">
<link rel="alternate" hreflang="x-default" href="https://algorithmdubai.com/preparing-for-school-in-dubai">
<meta property="og:locale" content="en_US">
```

### HEAD для русской версии /podgotovka-k-shkole-v-dubae (добавить в конец поля)

```html
<link rel="alternate" hreflang="ru" href="https://algorithmdubai.com/podgotovka-k-shkole-v-dubae">
<link rel="alternate" hreflang="en" href="https://algorithmdubai.com/preparing-for-school-in-dubai">
<link rel="alternate" hreflang="x-default" href="https://algorithmdubai.com/preparing-for-school-in-dubai">
<script>
document.addEventListener('DOMContentLoaded',function(){document.querySelectorAll('a').forEach(function(a){if(a.textContent.trim().toLowerCase()==='en')a.setAttribute('href','https://algorithmdubai.com/preparing-for-school-in-dubai');});});
</script>
```

### HTML-код статьи 2 (вставить целиком в блок T123)

```html
<!-- Algorithm Dubai · Preparing for School in Dubai (EN) · paste into the T123 HTML block on /preparing-for-school-in-dubai -->
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

<article class="alg-art" lang="en" itemscope itemtype="https://schema.org/Article">
<meta itemprop="headline" content="Preparing for School in Dubai: What Your Child Should Know at 5-6">

<p class="alg-byline"><span>Parent's guide</span> By the Algorithm Training Center team · Updated <time datetime="2026-11-26">26 November 2026</time></p>

<p class="alg-lead">In Dubai, "is my child ready for school?" is a harder question than back home. It's not only about reading and counting, but also about the language. Some families are preparing for a Russian first grade, others for Year 1 at a British school, and some want to keep both options open.</p>

<p>Here's which skills really matter by age 6, and how to build them without turning childhood into endless lessons.</p>

<figure class="alg-fig"><img src="https://algorithmdubai-production.up.railway.app/blog-images/kids-shapes-activity-with-parents.webp" alt="Children sorting coloured paper shapes at an open lesson while parents watch" width="960" height="540"><figcaption>School readiness isn't only reading and counting: it's also working in a group</figcaption></figure>

<nav class="alg-toc" aria-label="Contents">
<b>Contents</b>
<ol>
<li><a href="#when">When to start</a></li>
<li><a href="#checklist">School readiness checklist</a></li>
<li><a href="#international">Heading to an international school</a></li>
<li><a href="#russian-school">Heading to the Russian curriculum</a></li>
<li><a href="#home">7 habits for home</a></li>
<li><a href="#specialist">When to see a specialist</a></li>
<li><a href="#algorithm">School preparation at Algorithm</a></li>
<li><a href="#faq">FAQ</a></li>
</ol>
</nav>

<h2 id="when">When to start preparing</h2>
<p>Ideally a year before school, at 5 to 5.5. That's enough time to learn letters, reading and counting calmly, without rushing your child.</p>
<p>If your child goes to an English-speaking nursery, start with Russian even earlier. By age 5, many children in Dubai play and talk mostly in English, and Russian becomes the "home" language.</p>

<h2 id="checklist">Checklist: what your child should be able to do</h2>
<p>This is a guide, not an exam. If a skill isn't there yet, it's a reason to give it some attention, not a diagnosis.</p>

<div class="alg-cards">
<div class="alg-card"><b>Speech</b><ul><li>Retells a short story in their own words.</li><li>Makes up a 4-5 sentence story from a picture.</li><li>Pronounces the sounds of their first language correctly.</li><li>Asks questions and explains what they want.</li></ul></div>
<div class="alg-card"><b>Letters and reading</b><ul><li>Knows the letters and tells vowels from consonants.</li><li>Reads simple words syllable by syllable.</li><li>Writes their name in block letters.</li></ul></div>
<div class="alg-card"><b>Maths</b><ul><li>Counts to 20 and back, knows number bonds to 10.</li><li>Solves simple "more or less" and "add or take away" problems.</li><li>Knows basic shapes and finds their way around a page: top right, under the line.</li></ul></div>
<div class="alg-card"><b>Fine motor skills</b><ul><li>Holds a pencil correctly.</li><li>Traces outlines and colours inside the lines.</li><li>Cuts with scissors, models with clay, builds small construction sets.</li></ul></div>
<div class="alg-card"><b>Attention and behaviour</b><ul><li>Focuses on one task for 15-20 minutes.</li><li>Follows 2-3 step instructions.</li><li>Finishes what they start.</li><li>Copes calmly with losing a game.</li></ul></div>
<div class="alg-card"><b>Independence</b><ul><li>Dresses on their own, manages fasteners and shoes.</li><li>Packs their bag and keeps track of their things.</li><li>Can ask an adult for help.</li></ul></div>
</div>

<h2 id="international">If your child is going to an international school</h2>
<p>From the 2026-27 academic year, British schools in Dubai that start in September place new pupils by their age on 31 December: FS1 from age 3, FS2 from 4, Year 1 from 5.</p>
<p>The entrance assessment usually looks at whether your child:</p>
<ul>
<li>understands spoken English and simple instructions;</li>
<li>knows English letters and sounds, usually taught through phonics;</li>
<li>can count and understands basic maths concepts;</li>
<li>can communicate and work in a group.</li>
</ul>
<p>The most common difficulty for Russian-speaking children is the language, not the knowledge: a child can solve the problem but doesn't understand what's being asked. So preparing for an international school is mostly about English in real classroom situations: listening to the teacher, answering questions, working through tasks.</p>
<p>For more on choosing a school and admissions, read <a href="/how-to-choose-a-school-in-dubai">How to Choose a School in Dubai</a>.</p>

<h2 id="russian-school">If your child is following the Russian curriculum</h2>
<p>A Russian first grade expects children to read and write in Russian, and for a child growing up in an English-speaking environment that's a separate task. Children who speak Russian fluently at home often surprise their parents at assessment: their speaking is good, but sound analysis, reading and writing lag behind children of the same age in Russia.</p>
<p>Regularity matters here. Two or three sessions a week with a teacher do more than an intensive month just before school.</p>

<figure class="alg-fig"><img src="https://algorithmdubai-production.up.railway.app/blog-images/shkola-rossii-workbooks.webp" alt="Russian Year 1 workbooks: Russian language, maths and the world around us" width="960" height="540" loading="lazy"><figcaption>A Russian first grade expects children to read and write in Russian</figcaption></figure>

<h2 id="home">7 simple habits to build at home</h2>
<ol class="alg-steps">
<li><b>Read aloud every day</b> in the language that's harder to keep up. Talk about the story: "Why did the character do that?"</li>
<li><b>Play word games:</b> "name a word that starts with M", "what's the last sound in cat".</li>
<li><b>Count in everyday life:</b> plates on the table, steps, coins, cars in the car park.</li>
<li><b>Give multi-step tasks:</b> "take the book, put it on the table and call Dad".</li>
<li><b>Draw, model and cut out.</b> It's the best preparation for writing.</li>
<li><b>Teach them to finish things:</b> a completed puzzle, a finished drawing, toys put away.</li>
<li><b>Don't compare</b> your child with others. Bilingual children almost always have one language that develops faster, and that's normal.</li>
</ol>

<h2 id="specialist">When to see a specialist</h2>
<p>It's worth having your child seen by a teacher or speech therapist if:</p>
<ul>
<li>pronunciation problems are still noticeable at 5;</li>
<li>it's hard for them to focus even on something they enjoy;</li>
<li>they avoid drawing and any pencil tasks;</li>
<li>they mix languages so much that they're not understood in either.</li>
</ul>

<div class="alg-promo">
<p>Start with a free assessment at Algorithm: a teacher will check school readiness and your child's Russian and suggest the right preparation format.</p>
<a class="alg-btn" href="#reg">Book a free assessment</a>
</div>

<h2 id="algorithm">School preparation at Algorithm</h2>
<p>We run two school preparation formats for children from 5.5:</p>
<table class="alg-table">
<thead><tr><th>Format</th><th>When</th><th>What's included</th></tr></thead>
<tbody>
<tr><td><b>Saturdays</b></td><td>Saturday, 09:00-13:00</td><td>Reading and writing in Russian, maths, the world around us, speech development. A good fit if your child goes to an English-speaking nursery and you want to keep Russian going without overloading the week.</td></tr>
<tr><td><b>Five days a week</b></td><td>Monday-Friday, 09:00-13:00</td><td>All-round preparation, including for international school: Russian, maths, the world around us, speech and reading, plus extra English (Jolly Phonics, First Math, Storytelling).</td></tr>
</tbody>
</table>
<p>Both programmes follow the Russian federal education standard (FGOS). <a href="https://algorithmdubai.com/#programs">See all programmes</a>.</p>

<h2 id="faq">FAQ</h2>
<div class="alg-faq">
<details><summary>At what age should we start preparing for school?</summary><p>Ideally a year before school, at 5 to 5.5. If your child goes to an English-speaking nursery, keep up Russian from an earlier age.</p></details>
<details><summary>Should my child read before starting school?</summary><p>For a Russian first grade, reading syllable by syllable is expected. In the British system children learn to read in FS2 and Year 1 through phonics, but knowing letters and sounds gives them a confident start.</p></details>
<details><summary>How do I know if my child is ready for school?</summary><p>Use the checklist: speech, letters, counting, fine motor skills, attention and independence. A teacher's assessment gives an objective picture.</p></details>
<details><summary>Can we prepare for Russian and international school at the same time?</summary><p>Yes, with the right balance: core subjects in Russian plus regular English practice. That's how the five-day preparation at Algorithm works.</p></details>
<details><summary>What age do children start Year 1 in Dubai?</summary><p>From the 2026-27 academic year, schools that start in September admit children to Year 1 if they turn 5 by 31 December.</p></details>
</div>

<h2 id="sources">Sources</h2>
<div class="alg-sources">
<ul>
<li><a href="https://www.khaleejtimes.com/uae/dubai-school-admissions-khda-new-guide-age-cut-off?utm_source=algorithmdubai&utm_medium=referral&utm_campaign=blog_preparatory_en" target="_blank" rel="noopener">Khaleej Times</a>: new admission age rules for Dubai schools from 2026-27.</li>
</ul>
</div>

<div class="alg-final">
<p>Find out whether your child is ready for school with a free assessment at Algorithm Training Center.</p>
<a class="alg-btn" href="#reg">Book a free assessment</a>
</div>
</article>

<script type="application/ld+json">
{
 "@context": "https://schema.org",
 "@graph": [
  {
   "@type": "Article",
   "headline": "Preparing for School in Dubai: What Your Child Should Know at 5-6",
   "description": "A school readiness checklist for children aged 5-6: speech, reading, maths, English, attention and independence. How to prepare for Russian and international schools.",
   "inLanguage": "en",
   "datePublished": "2026-11-26",
   "dateModified": "2026-11-26",
   "mainEntityOfPage": "https://algorithmdubai.com/preparing-for-school-in-dubai",
   "image": "https://algorithmdubai-production.up.railway.app/blog-images/kids-shapes-activity-with-parents.webp",
   "author": {
    "@type": "Organization",
    "name": "Algorithm Training Center",
    "url": "https://algorithmdubai.com/"
   },
   "publisher": {
    "@type": "Organization",
    "name": "Algorithm Training Center",
    "url": "https://algorithmdubai.com/"
   }
  },
  {
   "@type": "BreadcrumbList",
   "itemListElement": [
    {
     "@type": "ListItem",
     "position": 1,
     "name": "Home",
     "item": "https://algorithmdubai.com/"
    },
    {
     "@type": "ListItem",
     "position": 2,
     "name": "Blog",
     "item": "https://algorithmdubai.com/blog"
    },
    {
     "@type": "ListItem",
     "position": 3,
     "name": "Preparing for School in Dubai",
     "item": "https://algorithmdubai.com/preparing-for-school-in-dubai"
    }
   ]
  },
  {
   "@type": "FAQPage",
   "mainEntity": [
    {
     "@type": "Question",
     "name": "At what age should we start preparing for school?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Ideally a year before school, at 5 to 5.5. If your child goes to an English-speaking nursery, keep up Russian from an earlier age."
     }
    },
    {
     "@type": "Question",
     "name": "Should my child read before starting school?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "For a Russian first grade, reading syllable by syllable is expected. In the British system children learn to read in FS2 and Year 1 through phonics, but knowing letters and sounds gives them a confident start."
     }
    },
    {
     "@type": "Question",
     "name": "How do I know if my child is ready for school?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Use the checklist: speech, letters, counting, fine motor skills, attention and independence. A teacher's assessment gives an objective picture."
     }
    },
    {
     "@type": "Question",
     "name": "Can we prepare for Russian and international school at the same time?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "Yes, with the right balance: core subjects in Russian plus regular English practice. That's how the five-day preparation at Algorithm works."
     }
    },
    {
     "@type": "Question",
     "name": "What age do children start Year 1 in Dubai?",
     "acceptedAnswer": {
      "@type": "Answer",
      "text": "From the 2026-27 academic year, schools that start in September admit children to Year 1 if they turn 5 by 31 December."
     }
    }
   ]
  }
 ]
}
</script>
<script>
(function(){
  var LANG={label:'RU',href:'https://algorithmdubai.com/podgotovka-k-shkole-v-dubae'};
  var FORMS={"Blog eng: program selection": "Blog eng prep: program selection", "Living in Dubai with kids: program selection": "Blog eng prep: program selection", "Blog eng: lesson": "Blog eng prep: lesson", "Living in Dubai with kids: lesson": "Blog eng prep: lesson", "Blog eng: consultation and dia": "Blog eng prep: consultation and dia", "Living in Dubai with kids: consultation and dia": "Blog eng prep: consultation and dia"};
  function fix(){
    document.querySelectorAll('a').forEach(function(a){
      if(a.textContent.trim().toLowerCase()===LANG.label.toLowerCase()){a.setAttribute('href',LANG.href);}
    });
    document.querySelectorAll('input[name="formname"]').forEach(function(cur){
      var f=cur.form; if(!f) return;
      var key=cur.getAttribute('data-alg-orig')||cur.value; var m=FORMS[key]; if(!m) return;
      f.querySelectorAll('input[name="formname"],input[name="tildaspec-formname"],input[name="programs"]').forEach(function(x){x.setAttribute('data-alg-orig',key);x.value=m;});
    });
  }
  if(document.readyState!=='loading'){fix();}else{document.addEventListener('DOMContentLoaded',fix);}
  window.addEventListener('load',fix);
})();
</script>
```

---

## Отчёт, который нужно вернуть

Для каждой статьи: опубликованный адрес, что сделано по шагам 1-11, что не получилось и почему (со скриншотом), значения formname во всех трёх формах. Отдельно: добавлен ли HEAD-код на обе русские страницы и работает ли переключатель языка в обе стороны.
