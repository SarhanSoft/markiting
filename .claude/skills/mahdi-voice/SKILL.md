---
name: mahdi-voice
description: Rewrite any Arabic content text (reel script, carousel slides, post caption) in Mahdi's own voice — short blunt hook, contrarian angle, no hype, exact steps instead of general phrases, his Kuwaiti dialect — using rules learned from his hand edits of AI drafts. Use when Mahdi pastes a draft or points to a file and asks to fix its style («حوّله لأسلوبي», «عدّله بأسلوبي», «نقّ النص», «خله يطلع مثل كلامي»), and as step 4 of the media-content skill. Also use to record a new edit of his into the style guide.
---

# Mahdi's voice

**Problem this solves:** AI drafts sound like every other AI script: hype hooks, general
benefits, a slogan at the end. Mahdi's edits show exactly how he rewrites that. This skill applies
his edits before he has to.

Paths are relative to the project root (the folder holding `خطة-المحتوى.md`).

## Read first

`references/style.md` — the rules, each with before/after evidence from his own edits.
Non-negotiable.

## Rewrite

Apply every rule of `references/style.md`, in this order:

1. **Hook** → one short blunt line, a verdict or a sharp question. No «يا جماعة», no stacked «؟!».
2. **Angle** → prefer the contrarian or uncomfortable one if the material allows it.
3. **Exaggeration** → delete it, and delete the closing hype or moral. End on the result.
4. **General phrases** → replace each with the exact step, tool, or scene.
5. **Dialect** → only words from his list; correct his typing slips (hamzas, joined words).
6. **Shape** → keep the timed blocks; the hook appears once; 30–40 s is his natural length.
7. **Confidentiality** → a client, employer or internal system named? Ask before keeping it.

Then read the hook alone: would a business owner stop scrolling on it? If not, rewrite it.

Never add facts, numbers or examples the draft does not have. If a rule needs a concrete detail
the draft lacks (rule 4), ask Mahdi for it in one question instead of inventing one.

## Deliver

- **Called by media-content** → return the rewritten text to that step.
- **Called directly** → reply with the rewritten text in the same shape as the input, then at
  most three short lines on the main changes. If the input was a file, edit it in place.

## Learn from his edits

When Mahdi edits a text this skill produced, or gives a before/after pair:

1. Compare the two and list what he changed.
2. A change that repeats an existing rule → add it as another example row under that rule.
3. A new kind of change → add a new rule with the pair as evidence, and tell him in one line.
4. Save the pair: the draft in `group N/`, his version in `group N/تنقية النص/`, same file name.
