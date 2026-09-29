# Mahdi's writing style — extracted from his own edits

**Evidence base:** `group 1/*.txt` are AI-drafted scripts; `group 1/تنقية النص/*.txt` are the same
scripts after Mahdi edited them by hand. Every rule below is a change he made himself. Re-derive
with: `diff "group 1/<file>" "group 1/تنقية النص/<file>"`.

`group 2/` holds AI drafts he has **not** edited yet, so they are not evidence of his voice. Use
them as test inputs: rewrite one and compare with his edit once he makes it.

## 1. Hooks: short, blunt, a claim or a sharp question — no hype

| AI draft | Mahdi's version |
|---|---|
| «يا جماعة، أحس البحث في جوجل صار أصعب من قبل. تكتب سؤال بسيط، وتطلع لك مليون نتيجة!» | «البحث في قوقل صار قديم» |
| «المعاملات - Transaction... درع البرمجة اللي يحمي بياناتك من الأخطاء!» | «Transaction درع المبرمج» |
| «for loop؟ للحين تستخدمها؟! في حلول أسهل بكثير!» | «هل For Loop صار قديم؟» |
| «الشطرنج لعبة عبقرية... بس ليش لازم تضحي عشان تفوز؟!» | «الشطرنج تعتمد على مبدأ إذا ما ضحيت ما تفوز» |

Rule: one short sentence, often a verdict («صار قديم») or a principle. No «يا جماعة», no stacked
«؟!», no «مليون».

## 2. Contrarian or uncomfortable angles are welcome

| AI draft | Mahdi's version |
|---|---|
| «تحتاج تكتب إيميل ممتاز؟ الذكاء الاصطناعي راح يكتبه لك باحترافية!» | «لا تكتب ايميل بنفسك للمدير او للعميل لانك ماراح توصل الفكرة ولا تخلي انطباع قوي» |
| «شلون تحل مشكلة تلقائية ما اشتغلت؟ عندنا الحل!» | «ليش المبرمجين يسوون BACK DOOR في تطبيقاتهم؟!» |

Rule: prefer the angle that challenges a habit or reveals a real engineering trade-off («لابد من
وجود باب خلفي يخلي المبرمج ينفذ الاكواد…») over a friendly promise.

## 3. Cut the exaggeration and the sales ending

- He deleted «بكثير», «خسائر كبيرة», «فقط!», «بسهولة!».
- He deleted closing hype and morals: «جربها!», «درس تعلمناه؟ بعض الأخطاء مو في الكود…»,
  «كود يشتغل لحاله، بيانات دقيقة…». Several scripts lost their whole last block.
- Rule: end on the result or the fact. At most one plain call to action, never a slogan.

## 4. Precise and concrete over general

| AI draft | Mahdi's version |
|---|---|
| «باقي نقاط الربط مثل POST وGET كانت تشتغل» | «POST وGET كانت تشتغل بس PUT وDELETE لا» |
| «حذف أو تعطيل WebDAVModule من إعدادات IIS» | «حذف WebDAVModule» |
| «يجمع البيانات، يتحقق منها، ويقفل الجلسة» | «يجمع البيانات، يدفع الشحنات الغير مدفوعة، ويقفل الجلسة» |
| «الذكاء الاصطناعي يصيغ لك الإيميل» | «اكتب محتوى الرسالة لـ CHAT GPT … يجهزلك الإيميل» |

Rule: name the exact method, tool, or step. Replace a list of abstract benefits with one real
scene: «يوم ثاني يجي المحاسب يشوف كل شي مكتمل، والموظف يبدأ جلسة جديدة».

## 5. Dialect

Gulf/Kuwaiti as he writes it: بس، شنو، شلون، هني، الحين، تبي، مو، ما نقدر، لابد، عشان، شي،
يجهزلك، بنص الليل، يا … يا. Do not add dialect words he never uses. His typing drops hamzas and
spaces («الي», «مانقدر», «اصلاح») — that is haste, not style: write them correctly.

## 6. Shape

- Timed blocks like his files: `(0-5 ثانية)`, `(6-15 ثانية)`, `(16-30 ثانية)`, `(31-40 ثانية)`.
- He removes the duplicated hook block the AI adds; the hook appears once.
- Scripts often end at 30 s once the ending hype is cut; 30–40 s is his natural length.

## 7. Red flag he does not catch himself

His edited scripts name a real system («Safe Logestic System»). Never name a client, employer
or internal system in content without asking him first.
