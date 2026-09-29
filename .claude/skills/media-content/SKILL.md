---
name: media-content
description: Create one piece of Mahdi's media content (a reel script or carousel text for TikTok / Instagram, Arabic, Kuwaiti dialect) — find or take an idea, judge it against his content plan, write it, then rewrite it in his own voice learned from his edited scripts. Use when Mahdi gives a topic («اكتب عن…», «سوّ محتوى عن…»), asks for ideas («اعطني فكرة», «ابحث عن شي ننشره»), asks to be interviewed for one («اسألني»), shares a trend or a claim to answer, or asks to critique an AI tool or plugin for content.
---

# Media content

**Problem this solves:** an AI-drafted script sounds like every other AI script — hype hooks,
general benefits, a slogan at the end. Mahdi's own edits show exactly how he rewrites that
(the `mahdi-voice` skill). This skill applies his edits before he has to.

Paths are relative to the project root (the folder holding `خطة-المحتوى.md`): locally
`C:\Users\Mahdi\Documents\Marketing course`, in a cloud session the repository root.

## Read first

1. `خطة-المحتوى.md` — the ten topics, what changes in each, and which suit the educational start.
2. `نتائج-البحث.md` — facts and numbers already gathered, with sources.

## 1. Get the idea

Three ways in; take the one Mahdi asks for:

- **He gives a topic** → go to step 2 with it. If it needs facts you do not have, launch one
  `content-researcher` agent in `topic` mode with it.
- **He asks you to ask him** («اسألني», «طلّع مني فكرة») → ask up to three short questions at
  once, each tied to a different ✅ topic of the plan and aimed at something he lived, not an
  opinion. Examples: «شنو آخر مشكلة واجهتك بالـ ERP وما حلها الذكاء الاصطناعي؟», «أي ميكانيكية
  بلعبة لعبتها مؤخراً ضايقتك؟», «أي أداة ذكاء اصطناعي جربتها هالأسبوع؟». His answer becomes the
  topic; research it as above if needed.
- **He asks you to find one** → launch `content-researcher` agents in `discover` mode **in
  parallel**, one per lens. The lens is whatever he names (a topic number, a field, a platform,
  a news event); if he names none, use three: `trend`, `gaps`, `claims`. Merge the results,
  drop duplicates, and bring the best **three to five**, each in two lines: what it is, which
  topic of the plan it fits, and the source link. Stop and let him choose unless he asked you
  to choose.

## 2. Judge it before writing

Answer each in one line; reject the idea if any answer is "no":

- **Topic:** which of the ten topics in `خطة-المحتوى.md` does it belong to?
- **Phase:** does that topic suit the educational start (the ✅ column)? If ❌, say it waits.
- **AI test:** could anyone with the same AI make this within a month? If yes, what makes
  Mahdi's version different — his experience, a test he ran, his accounting + systems angle?
- **Proof:** what real example, test or number carries it? Never invent one. If it needs his
  experience, ask him for the example in one question.
- **Confidentiality:** does it touch a client, employer or internal system by name? Ask first.

## 3. Write the draft

Arabic, Kuwaiti dialect, in his timed-block shape:

```
(0-5 ثانية)   hook — one short verdict or sharp question
(6-15 ثانية)  the situation or the claim, concretely
(16-30 ثانية) what actually happens / the test / the method
(31-40 ثانية) the result — optional, often not needed
```

For a **claim or tool critique** (topic 1, AI tools), use: المقولة المنتشرة → تجربتي بالضبط →
النتيجة → حكمي وسببه. Criticise the tool, never the people who promote it; say what is good in
it if anything; state the test date, because these tools change within weeks. Do not judge a
tool you have not tested or researched — say what is unknown.

## 4. Rewrite it in his voice

Apply the `mahdi-voice` skill to the draft. Do not skip it, even when the draft already reads well.

## 5. Deliver

Save to `محتوى/<YYYY-MM-DD>-<short-english-slug>.md` (create the folder if missing), in this shape:

```markdown
---
التاريخ: <YYYY-MM-DD>
الموضوع: <number and name from the plan>
المرحلة: تثقيفية | مؤجلة
المصدر: <Mahdi | link>
---

# <title in Arabic>

## النص
(0-5 ثانية)
«…»
…

## نص المنشور
<one or two lines, the search keyword first> + 3–5 hashtags

## ملاحظات
- لماذا يناسب الخطة: <one line>
- الدليل: <the test, example, or source>
- ما لم يُتحقق منه: <anything unverified>
```

Check line starts: if `~/.claude/skills/owner-docs-style/scripts/check_line_start.py` exists, run
it on the file and fix every flagged line; if it does not (cloud sessions), check by eye that no
Arabic prose line starts with a Latin word, and rephrase any that does. Tell Mahdi in chat,
briefly and in Arabic: the hook, the topic, and anything he must confirm.
