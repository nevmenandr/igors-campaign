# Реконструкция перевода «Слова о полку Игореве»

Экспериментальный проект по восстановлению идеального современного перевода «Слова о полку Игореве».

---

## О проекте

Этот проект представляет собой **эксперимент** по применению методов **лингвистической реконструкции** к переводам «Слова о полку Игореве». Я не ставлю академических целей, это попытка проверить, можно ли, подобно тому как сравнительное языкознание восстанавливает праязыки на основе языков-потомков, восстановить «идеальный» вариант перевода на современный русский язык, сравнивая множество уже существующих переводов.

### Исходные данные

Материалом для реконструкции служит мой **Параллельный корпус переводов «Слова о полку Игореве»**: [nevmenandr.net/slovo](https://nevmenandr.net/slovo). Корпус включает **более 100 переводов** на русский язык (а также переводы на другие языки), выполненных в XIX–XXI веках.

## Метод реконструкции

Основная идея проекта — провести **аналогию** между:

- **Языками-потомками** (например, русский, болгарский, польский) и **переводами** «Слова»
- **Праязыком** (например, общеиндоевропейским) и **гипотетическим «идеальным» вариантом** перевода

В классическом сравнительно-историческом языкознании реконструкция основывается на нескольких принципах. Мы применяем их к материалу переводов:

### 1. Принцип большинства (от разнообразия к единообразию)
Если в большинстве переводов встречается одна форма, а в нескольких — другие, более подходящим признаётся **наиболее частотный** вариант. 

### 2. Принцип свободной дистрибуции
Из двух элементов более подходящим для реконструируемого признаётся тот, который имеет **более широкое распространение** (встречается в большем числе переводов).

### 3. Принцип дробления
Если в одних переводах некоторая форма сохраняется как одна, а в других распадается на несколько вариантов, то **отсутствие дробления** считается признаком правильности выбора.

### 4. Ареальный принцип
Сравниваются **центральные** (академические, филологические) и **периферийные** (поэтические, стилизованные, экспериментальные) переводы. Если необычный вариант встречается только в периферийных версиях — он, вероятно, является авторским окказионализмом, а не отражением идеального перевода. Общие для центра и периферии формы считаются более надёжными.

### 5. Учёт диахронической типологии
Мы учитываем, как менялись значения слов с течением времени. Например, древнерусское *трудный* означало «тяжёлый, горестный», а не «сложный». Поэтому буквальный перевод «трудные повести» сегодня был бы понят неверно — мы выбираем семантически адаптированный вариант **«печальные повести»**.

Более подробно с принципами лингвистической реконструкции можно ознакомиться в [этом файле](reconstruction.txt).

---

## Как устроен сайт

Текст «Слова о полку Игореве» разбит на **218 фрагментов**. Для каждого фрагмента:

1. **Сопоставляются** все доступные переводы
2. **Применяются** описанные выше принципы для выбора наиболее подходящего варианта
3. **Формулируется** итоговый реконструированный текст на современном русском языке
4. **Приводятся** пояснения к каждому выбору (почему именно этот вариант был признан наиболее вероятным)

### Пример реконструкции

**Исходный древнерусский текст:**
> Не лѣпо ли ны бяшетъ, братіе, начяти старыми словесы трудныхъ повѣстій о пълку Игоревѣ, Игоря Святъславлича?

[Выборка переводов в корпусе](https://nevmenandr.net/cgi-bin/slovo.py?it=b1&it=b2&it=b3&it=b4&it=b5&it=b6&it=b7&it=b8&it=b9&it=ba&it=bb&it=bc&it=bd&it=be&it=bg&it=bh&it=bi&it=bk&it=bk1&it=bl&it=bm&it=bn&it=bo&it=bp&it=bq&it=br&it=bs&it=bt&it=bu&it=bv&it=bw&it=bx&it=by&it=bz&it=c1&it=c2&it=c5&it=c6&it=c7&it=c8&it=c9&it=ca&it=cb&it=cc&it=cd&it=ce&it=cf&it=cg&it=ch&it=ci&it=cy&it=cz&it=d1&it=d2&it=d3&it=e1&it=e2&it=e3&it=e9&it=eh&it=ek&it=en&it=ep&it=er&it=es&it=f1&it=f2&it=f3&it=f4&it=f5&it=f6&it=f7&it=f8&it=f9&it=fa&it=fb&it=fc&it=fd&it=fe&it=ff&it=fg&it=fh&it=fi&it=fj&it=fk&it=g1&it=g2&it=g3&it=g4&it=g5&it=g6&it=g7&it=g8&it=g9&it=ga&it=gb&it=gc&it=gd&it=ge&it=gf&it=gg&it=gh&it=gi&it=gj&it=gk&it=gl&it=gt&it=gv&it=gw&it=gx&it=gy&it=gz&fragm=1)

**Наши шаги (кратко):**
- «Не лѣпо ли» → в ~25 переводах «не пристало ли» (принцип большинства)
- «ны» → «нам» (в ~75 переводах, принцип свободной дистрибуции)
- «братіе» → «братья» (в ~55 переводах, принцип отсутствия дробления)
- «словесы» → «словами» (прямой эквивалент, а не «слогом/складом», принцип дробления)
- «трудныхъ» → «печальные» (учёт изменения значения слова)
- «пълку» → «поход» (в ~60 переводах, семантическая адаптация)

**Реконструированный вариант:**
> **Не пристало ли нам, братья, начать старыми словами печальные повести о походе Игоревом, Игоря Святославича?**

---

## Статус проекта

Проект **не является научным исследованием**. Это **эксперимент** на стыке лингвистики, художественного перевода и компьютерных наук (в области применения LLM). 

Все промежуточные данные и пояснения открыты для проверки и обсуждения.

---

## Как использовать сайт

- **Навигация по фрагментам**: Выберите номер фрагмента (1–218) в меню.
- **Сравнение переводов**: Для каждого фрагмента отображаются все переводы, использованные для реконструкции.
- **Обоснование**: Под итоговым текстом приведены пояснения о том, по какому принципу был выбран каждый элемент.
- **Исходный код**: Весь код проекта доступен в репозитории, вы можете запустить реконструкцию на своих данных.

---

## Источники и ссылки

- **Параллельный корпус переводов «Слова о полку Игореве»**: [nevmenandr.net/slovo](https://nevmenandr.net/slovo) (2007)
- **Статья о корпусе** [Параллельный корпус переводов «Слова о полку Игореве» как проект](https://nevmenandr.github.io/portfolio/assets/pdf/cgi2025-1-spi.pdf), DOI: 10.31860/cgi-2025-1-60-69 (2025) 
- **Принципы лингвистической реконструкции**: [файл](reconstruction.txt) или [внешний источник](https://studfile.net/preview/4513885/)
- [Праиндоевропейский язык: реконструкция или химера?](https://slovokod.ru/pie-kritika/)

---

## Лицензия

Весь текст, данные и результаты реконструкции распространяются под лицензией [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). Это означает, что вы можете свободно использовать, изменять и распространять материалы проекта при условии указания авторства.

---

## Автор

[Борис Орехов](https://nevmenandr.github.io/): 

<div style="margin-bottom: 10px;">
  <a href="https://bsky.app/profile/nevmenandr.bsky.social">
    <img src="https://img.shields.io/badge/Bluesky-0285FF?style=for-the-badge&logo=Bluesky&logoColor=white" alt="Bluesky">
  </a>
  <a href="https://mastodon.social/@nevmenandr">
    <img src="https://img.shields.io/badge/-MASTODON-%232B90D9?style=for-the-badge&logo=mastodon&logoColor=white" alt="Mastodon">
  </a>
  <a href="https://t.me/schonenrede">
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>
  <a href="https://x.com/nevmenandr">
    <img src="https://img.shields.io/badge/X-%23000000.svg?style=for-the-badge&logo=X&logoColor=white" alt="X">
  </a>
  <a href="https://www.youtube.com/@schonenrede/">
    <img src="https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white" alt="YouTube">
  </a>
</div>

<div style="margin-bottom: 10px;">
  <a href="https://hse-ru.academia.edu/BorisOrekhov">
    <img src="https://img.shields.io/badge/academia-41454A?style=flat-square&logo=academia&logoColor=white" alt="Academia">
  </a>
  <a href="https://arxiv.org/search/cs?searchtype=author&query=Orekhov,+B">
    <img src="https://img.shields.io/badge/-arxiv-B31B1B?style=flat-square&logo=arxiv&logoColor=white" alt="arXiv">
  </a>
  <a href="https://dev.to/nevmenandr">
    <img src="https://img.shields.io/badge/dev-000000?style=flat-square&logo=dev.to&logoColor=white" alt="Dev.to">
  </a>
  <a href="https://www.scopus.com/authid/detail.uri?authorId=57190401804">
    <img src="https://img.shields.io/badge/elsevier-FF6C00?style=flat-square&logo=elsevier&logoColor=white" alt="Elsevier">
  </a>
  <a href="https://habr.com/ru/users/nevmenandr/">
    <img src="https://img.shields.io/badge/habr-65A3BE?style=flat-square&logo=habr&logoColor=white" alt="Habr">
  </a>
  <a href="https://huggingface.co/nevmenandr">
    <img src="https://img.shields.io/badge/huggingface-FFD21E?style=flat-square&logo=huggingface&logoColor=white" alt="Hugging Face">
  </a>
  <a href="https://orcid.org/0000-0002-9099-0436">
    <img src="https://img.shields.io/badge/orcid-A6CE39?style=flat-square&logo=orcid&logoColor=white" alt="ORCID">
  </a>
  <a href="https://osf.io/phy74/">
    <img src="https://img.shields.io/badge/osf-2CB9F1?style=flat-square&logo=osf&logoColor=white" alt="OSF">
  </a>
</div>

<div>
  <a href="https://pypi.org/user/nevmenandr/">
    <img src="https://img.shields.io/badge/pypi-3775A9?style=flat-square&logo=pypi&logoColor=white" alt="PyPI">
  </a>
  <a href="https://researchgate.net/profile/Boris-Orekhov">
    <img src="https://img.shields.io/badge/researchgate-00CCBB?style=flat-square&logo=researchgate&logoColor=white" alt="ResearchGate">
  </a>
  <a href="https://www.semanticscholar.org/author/Boris-V.-Orekhov/2080424505">
    <img src="https://img.shields.io/badge/semanticscholar-1857B6?style=flat-square&logo=semanticscholar&logoColor=white" alt="Semantic Scholar">
  </a>
  <a href="https://ru.wikipedia.org/wiki/%D0%A3%D1%87%D0%B0%D1%81%D1%82%D0%BD%D0%B8%D0%BA:Nevmenandr">
    <img src="https://img.shields.io/badge/wikipedia-000000?style=flat-square&logo=wikipedia&logoColor=white" alt="Wikipedia">
  </a>
</div>
