# Tests: without the skill vs with the skill

🇷🇺 [Русская версия](README.ru.md)

Method: 4 cases, same model (Claude Sonnet), same question. The only difference is that on the second run the model reads `SKILL.md` first. Answers were given in Russian. Below they are translated and shortened, keeping the substance.

**To be honest up front:** a plain model already saves money. It will also say "don't buy the 30k thing". The difference is *how it thinks*:

| | Without skill | With skill |
|---|---|---|
| Starts with | "Buy the same thing, cheaper" | "What functions do you actually need?" |
| Free option from stuff at home | Sometimes, in passing | Always, first |
| When to buy the proper thing | Vague | Concrete triggers |
| First step | "Start with a tripod and lamps" (i.e. go shopping) | Something to do today, for free |
| Dangerous cases | Warns | Says "don't cut corners here", then tries to shrink the problem itself |

---

## Case 1. Overhead camera for drawing tutorials (30,000 ₽ ≈ $330)

> "I want to film my desk from above for drawing tutorials. People recommend an overhead camera with a boom arm for 30k plus lights. Too expensive."

**❌ Without skill.** Says to shoot on your phone. Then a shopping list: a boom tripod (800–2,000 ₽) or a tripod with a horizontal column (1,500–3,000 ₽), two LED panels (2–3k), a lav mic (1k). "Tape it to a shelf" gets one line as "janky but works". Final advice: *"Start with a tripod and lamps"*, so step one is going shopping.

**✅ With skill.**
> **What you actually need:** a strict top-down view, a camera that stays still, even light with no glare.
> 🪛 **Free:** tape or zip-tie the phone to a mop handle clamped to a chair back. Diffuse a desk lamp with baking paper. A white sheet or foil on the side replaces a second lamp.
> *Downsides:* the phone may fall, so keep something soft underneath. The jank stays out of frame, only the desk is visible.
> 🛒 **Under 3,000 ₽:** a used clamp tripod, a 5000 K LED bulb so paint colors look right.
> 💰 **Buy the real thing** when you shoot several videos a week and setup eats your time, or the videos start earning.
> **Start with:** today, tape the phone to a mop, cover the lamp with baking paper and shoot a 30-second test.

---

## Case 2. Family photo storage (Synology NAS for 50,000 ₽ ≈ $550)

> "I want storage for family photos, ~2 TB, everyone uploads from their phones. People recommend a Synology NAS, about 50k. Too expensive."

**❌ Without skill.** Three paths by price: a cloud plan (800–1,000 ₽/mo), *buy* a used mini PC and two drives (20–25k) running Immich, *buy* an external 4 TB drive. Good point that RAID isn't a backup. Final advice: *"Don't want to tinker, go cloud. Like tinkering, option 2."*

**✅ With skill.**
> **What you actually need:** store 2 TB, auto-upload from the family's phones, access from anywhere, don't lose anything. The software does the syncing. Most of the Synology price is the brand.
> 🪛 **Free:** an old laptop lying around plus drives from previous computers. Immich is free, and so is Tailscale for remote access.
> *Downsides:* a single drive with no copy can die with all your photos, and the laptop is noisy.
> 🛒 **~5,000 ₽:** a used mini PC or Raspberry Pi if you have no spare hardware.
> 💰 **Don't cut corners on backups:** family photos can't be recovered, so follow 3-2-1 with an offsite cloud copy. Get a NAS when you don't want to be the admin.
> **Start with:** find an old laptop, run Immich in Docker, connect your own phone as a test.

---

## Case 3. Standing desk (35,000 ₽ ≈ $385)

> "My back hurts, I want to work standing. An electric standing desk costs 35k, too expensive."

**❌ Without skill.** A list of purchases: a desktop converter (5–15k), a manual crank frame (12–20k), a used electric desk (10–15k), an anti-fatigue mat. DIY comes second in the list: *"a box or an IKEA LACK stool, 1–3k"*.

**✅ With skill.**
> **What you actually need:** a surface at elbow height, a screen at eye level, changing posture. *You don't need a motor. You need height.*
> 🪛 **Free:** an ironing board at max height, a dresser or the kitchen counter. Laptop on a stack of books, keyboard lower. A phone timer: 30–45 min standing.
> 🛒 **Under 3,500 ₽:** a used desktop riser, a piece of camping foam instead of a mat.
> 💰 **Buy the real thing** if after 2–3 weeks you actually stand 2+ hours a day.
> **No corner-cutting:** if the pain radiates into your leg, see a doctor. A desk won't fix that.
> **Start with:** today, work at the kitchen counter for 30 minutes.

---

## Case 4. Heater in a shed (15,000 ₽ wiring job). The safety boundary

> "An electrician wants 15k to run a dedicated line to my shed for a 2 kW heater, 25 m away. Maybe cheaper with extension cords?"

This case checks that ingenuity doesn't turn into stupidity.

**❌ Without skill.** Also rejects extension cords: 9 A, household 0.75 mm² cable melts. Suggests buying the cable and breaker yourself and paying the electrician only to connect it, about 8–10k.

**✅ With skill.**
> 🪛 **Free: extension cords, no, don't cut corners here.** Sustained load, dry wood, nobody watching. You can't solve this with stuff at hand.
> But you can *shrink the problem*: insulate the shed and heat only the work area, or use a 1 kW heater instead of 2 kW.
> 🛒 Buy the 3×2.5 mm² cable, C16 breaker and RCD yourself, dig the trench yourself, pay the electrician only for the connection.
> **Start with:** call two electricians and ask "how much for installation if I bring the cable and breaker?"

With the skill the model held the safety line and found a move the plain model didn't: shrink the problem itself.

---

## Takeaway

Without the skill, the model saves money with a **discount**: the same thing, cheaper. With the skill, it saves money with **ingenuity**: first work out what you really need, then cover it with what's already at home. Buying becomes the last step, not the first.

*Tested 2026-11-02, Claude Sonnet, one run per variant. A demo, not a benchmark.*
