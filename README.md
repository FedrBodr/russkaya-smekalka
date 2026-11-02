# 🪛 Русская смекалка / Russkaya Smekalka

> **Экономит не токены, а ваши деньги.**
> **Saves your money, not tokens.**

**[🇷🇺 Русский](#-русский) · [🇬🇧 English](#-english)**

---

## 🇷🇺 Русский

### Экономит не токены, а ваши деньги

Сейчас все заморочены экономией токенов. А по-настоящему стоит экономить тот ресурс, которого вы в жизни тратите больше всего: деньги. ИИ за них не платит, ему всё равно, сколько стоит его совет. Поэтому по умолчанию он легко подталкивает к покупке: «возьми вот это за 30 тысяч, и ещё вот это».

Этот скилл работает против этого. Он проверяет, не хочет ли ИИ развести вас на капитализм, и сначала ищет решение, которое дешевле или вообще бесплатное.

Скилл для Claude Code и других ИИ-агентов. Он учит агента отвечать на «купи камеру за 30 тысяч» так: «Погоди. Телефон есть? Швабра есть? Лампа есть? Значит, у тебя уже есть верхняя камера со светом».

### Зачем

Обычный ИИ на «это слишком дорого» предлагает то же самое, только подешевле. Это скидка, а не смекалка. Скилл меняет порядок мыслей:

1. **Разобрать покупку на функции.** Что мы на самом деле покупаем?
2. **Провести инвентаризацию.** Что уже лежит дома?
3. **Закрыть каждую функцию подручным.** Лампа, вытяжка, скотч, стопка книг, старый телефон, гладильная доска.
4. **Дать лестницу решений:** 🪛 0 ₽ → 🛒 копейки → 💰 когда всё-таки купить нормальное.
5. **Закончить первым шагом,** который можно сделать сегодня бесплатно.
6. **Не экономить там, где опасно:** электричество, газ, тормоза, здоровье, данные.

### Пример (реальный тест)

> **Вопрос:** «Болит спина, хочу работать стоя. Стол с электроподъёмником стоит 35 тысяч, это дорого».

| ❌ Без скилла | ✅ Со скиллом |
|---|---|
| Купи надстройку за 5–15 тысяч, каркас за 12–20 тысяч или б/у электростол за 10–15 тысяч. Плюс коврик. | *Электромотор не нужен. Нужна высота.* Гладильная доска на максимуме или кухонная стойка, ноутбук на стопке книг, таймер на 30–45 минут. **0 ₽.** Если через 2–3 недели реально стоишь по 2+ часа в день, тогда покупай стол. Если боль отдаёт в ногу, иди к врачу. **Начни с:** сегодня 30 минут поработай на кухонной стойке. |

👉 **Ещё 4 кейса с полными ответами** (камера сверху, хранилище фото вместо NAS, проводка в сарай): [examples/README.ru.md](examples/README.ru.md)

### Установка

**Claude Code (плагин):**
```
/plugin marketplace add FedrBodr/russkaya-smekalka
/plugin install russkaya-smekalka@russkaya-smekalka
```

**Вручную (Claude Code, Codex и другие агенты со skills):**
```bash
git clone https://github.com/FedrBodr/russkaya-smekalka
cp -r russkaya-smekalka/skills/russkaya-smekalka ~/.claude/skills/
```

Скилл срабатывает сам на «дорого», «подешевле», «на коленке», «бюджетно» или «без покупки». Можно позвать и явно: *«включи русскую смекалку»*.

### Контрибьютинг

Знаешь лайфхак «из говна и палок», который реально работает? Присылай PR в таблицу приёмов в [`SKILL.md`](skills/russkaya-smekalka/SKILL.md). Условия: лайфхак проверен в жизни и никого не убьёт.

---

## 🇬🇧 English

### Saves your money, not tokens

Everyone is obsessed with saving tokens. But the resource worth saving is the one you spend most in real life: money. The AI doesn't pay for its advice, so it doesn't care what that advice costs you. By default it nudges you to buy: "get this for $330, and this too".

This skill pushes back. It checks whether your AI is upselling you on consumerism, and finds a cheaper or free solution first.

An agent skill for Claude Code and other AI agents. *Smekalka* is the Russian word for street-smart ingenuity: the art of solving a problem with a mop handle, tape and whatever is lying around, instead of buying the "proper" thing.

Ask it "the overhead camera rig costs $330, too expensive", and it answers: "Wait. Got a phone? A mop? A desk lamp? Then you already own an overhead camera with lighting".

### Why

Ask a regular AI "this is too expensive" and it suggests the same thing, cheaper. That's a discount, not ingenuity. This skill changes the order of thinking:

1. **Break the purchase into functions.** What are you actually paying for?
2. **Take inventory.** What's already at home?
3. **Cover each function with stuff at hand.** A lamp, a kitchen hood, tape, a stack of books, an old phone, an ironing board.
4. **Give a cost ladder:** 🪛 free → 🛒 pocket change → 💰 when to actually buy the proper thing.
5. **End with a first step** you can take today, for free.
6. **Never cut corners where it's dangerous:** electricity, gas, brakes, health, data.

### Example (real test)

> **Question:** "My back hurts, I want to work standing. An electric standing desk costs 35k ₽ (~$385), too expensive."

| ❌ Without skill | ✅ With skill |
|---|---|
| Buy a desktop converter (5–15k), a manual crank frame (12–20k), or a used electric desk (10–15k). Plus a mat. | *You don't need a motor. You need height.* Ironing board at max height or the kitchen counter, laptop on a stack of books, a 30–45 min timer. **Free.** If after 2–3 weeks you actually stand 2+ hours a day, buy the desk. If the pain radiates into your leg, see a doctor. **Start with:** work at the kitchen counter for 30 minutes today. |

👉 **4 more cases with full answers** (overhead camera, family photo storage instead of a NAS, wiring a shed): [examples/README.en.md](examples/README.en.md)

### Install

**Claude Code (plugin):**
```
/plugin marketplace add FedrBodr/russkaya-smekalka
/plugin install russkaya-smekalka@russkaya-smekalka
```

**Manual (Claude Code, Codex and other agents that support skills):**
```bash
git clone https://github.com/FedrBodr/russkaya-smekalka
cp -r russkaya-smekalka/skills/russkaya-smekalka ~/.claude/skills/
```

It triggers on "too expensive", "cheaper", "budget", "DIY", "hack" or "without buying", in Russian or English. You can also call it explicitly: *"use russkaya smekalka"*. Answers come in the language you ask in.

### Contributing

Got a duct-tape hack that actually works? Send a PR to the tricks table in [`SKILL.md`](skills/russkaya-smekalka/SKILL.md). Rules: it's proven in real life and it won't kill anyone.

---

License: MIT · Structure: `skills/russkaya-smekalka/SKILL.md` (the skill) · `examples/` (tests) · `.claude-plugin/` (plugin manifest)
