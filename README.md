# 🪛 Русская смекалка

Скилл для Claude Code и других агентов. Он делает из ИИ человека, который на «купи камеру за 30 тысяч» отвечает: «Погоди. Телефон есть? Вытяжка есть? Значит, у тебя уже есть верхняя камера со светом».

## Зачем

Спросите обычного ИИ «это слишком дорого, что делать?», и он предложит купить то же самое, только подешевле. Этот скилл меняет порядок мыслей:

1. **Разобрать покупку на функции.** Что мы на самом деле покупаем?
2. **Провести инвентаризацию.** Что уже лежит дома?
3. **Закрыть каждую функцию подручным.** Лампа, вытяжка, скотч, стопка книг, старый телефон.
4. **Дать лестницу решений:** 0 ₽ → копейки → когда всё-таки купить нормальное.
5. **Честно сказать про риски.** Там, где экономить нельзя (электричество, газ, тормоза, здоровье, данные), скилл так и говорит: «тут не экономим».

## Пример

> **Ты:** Хочу снимать стол сверху для туториалов, советуют камеру с кронштейном за 30 тысяч. Это бред какой-то.
>
> **Агент со скиллом:**
> Что на самом деле нужно: вид сверху, неподвижность, ровный свет.
> 🪛 **0 ₽:** телефон кладём на решётку вытяжки камерой вниз, светит лампа вытяжки, стол ставим под ней. Блики гасим бумагой для выпечки на лампе.
> 🛒 **~300 ₽:** держатель-прищепка для телефона.
> 💰 **Купить нормальное**, если снимаешь каждый день и на кухне невозможно.
> **Начни с:** пробный ролик сегодня вечером.

## Установка

**Claude Code (как плагин):**

```
/plugin marketplace add FedrBodr/russkaya-smekalka
/plugin install russkaya-smekalka@russkaya-smekalka
```

**Вручную (Claude Code, Codex и другие агенты со skills):**

```bash
git clone https://github.com/FedrBodr/russkaya-smekalka
cp -r russkaya-smekalka/skills/russkaya-smekalka ~/.claude/skills/
```

После установки скилл срабатывает сам на фразы вроде «дорого», «подешевле», «на коленке», «бюджетно» или «без покупки». Можно позвать и явно: «включи русскую смекалку».

## Структура

```
skills/russkaya-smekalka/SKILL.md   # сам скилл
.claude-plugin/                     # манифест плагина Claude Code
```

## Контрибьютинг

Знаешь классный лайфхак «из говна и палок»? Присылай PR в таблицу приёмов в `SKILL.md`. Условия: лайфхак проверен в жизни и никого не убьёт.

---

## English

**Russkaya Smekalka** ("Russian ingenuity") is an agent skill for budget hacks. When something is "too expensive", the agent breaks the purchase down into the functions you actually need. Then it checks what you already own and covers each function with household items. It answers with a cost ladder: free → pocket change → when to actually buy the proper thing. It refuses to cut corners on safety-critical stuff (electricity, gas, brakes, health, data).

Install: `/plugin marketplace add FedrBodr/russkaya-smekalka`, or copy `skills/russkaya-smekalka` into `~/.claude/skills/`.

License: MIT.
