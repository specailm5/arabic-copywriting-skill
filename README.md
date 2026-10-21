# مهارة الإعلان والكتابة التسويقية
### (Arabic Copywriting & Advertising Skill)

<p align="center">
  <a href="https://github.com/specailm5/arabic-copywriting-skill/blob/master/LICENSE"><img alt="License" src="https://img.shields.io/github/license/specailm5/arabic-copywriting-skill?style=flat-square"></a>
  <a href="https://github.com/specailm5/arabic-copywriting-skill/commits/master"><img alt="Last commit" src="https://img.shields.io/github/last-commit/specailm5/arabic-copywriting-skill?style=flat-square"></a>
  <a href="https://specailm5.github.io/arabic-copywriting-skill/"><img alt="Docs" src="https://img.shields.io/badge/docs-live-brightgreen?style=flat-square"></a>
  <img alt="Agent Skills" src="https://img.shields.io/badge/Agent%20Skills-compatible-5B21B6?style=flat-square">
</p>

**Arabic copywriting skill for AI agents** — defines the audience and objection, builds the insight, big idea, benefit and proof, writes headlines, body copy, CTAs and slogans, and plans campaigns without manipulation: `«الحل الأمثل لحياتك»` ← `«فاتورتك أقل ٢٠٪ في ٣ دقائق»`. Works with Claude Code, Codex, Antigravity and VS Code agent harnesses.

🔗 **الموقع المرجعي (الفكرة والصنعة والحملة والنماذج): [specailm5.github.io/arabic-copywriting-skill](https://specailm5.github.io/arabic-copywriting-skill/)**

> مهارة برمجية ولغوية لنماذج الذكاء الاصطناعي والمحررات الذكية (Codex، Claude Code، Antigravity IDE، VS Code Agent Harness) لكتابة الإعلان العربي وتحريره وتقييمه، استناداً إلى **«فن الإعلان»** لأحمد فاربي، و**«الإعلان الفعال»** لعلي فلاح الزعبي.

---

## 📖 ما هي المهارة؟

أكثر الإعلانات العربية تقول «نحن الأفضل» ولا تقول لماذا، ولا لمن، ولا ما الذي يحدث لو جرّبت. والنتيجة نصّ منمق بلا فكرة.

تُمكِّنُ هذه المهارةُ الوكيلَ الذكيَّ من:

1. **تحديد الجمهور** والاعتراض قبل الكتابة.
2. **تحويل الميزة إلى فائدة**، والفائدة إلى وعد.
3. **بناء الفكرة الكبرى** واختبارها.
4. **كتابة العنوان** باثنتي عشرة صيغة.
5. **بناء النص** على AIDA، مع دليل واعتراض وCTA.
6. **كتابة الشعار** والوصف وصفحة الهبوط والبريد.
7. **تقييم الإعلان** في ثمانية محاور، مع سلم خطورة.

**القواعد الأربع:**
> **فكرة واحدة. فائدة واضحة. دليل صادق. ودعوة إلى فعل.**

---

## 📂 بنية المهارة ومكوناتها

<pre dir="rtl"><code>
arabic-copywriting-skill/
│
├── skills/arabic-copywriting-skill/          # المهارة (تركيب Agent Skills القياسي)
│   ├── SKILL.md                              # الدليل الأساسي: من الجمهور إلى الحملة
│   ├── references/                           # المراجع التفصيلية
│   │   ├── audience_insight.md               # الجمهور، الرحلة، الاعتراضات
│   │   ├── big_idea.md                       # الفائدة، الفكرة، الوعد، الدليل
│   │   ├── copy_craft.md                     # AIDA، العنوان، النص، CTA
│   │   └── campaign_ethics.md                # الموجز، الوسائط، القياس، الأخلاق
│   └── examples/                             # النماذج والتمارين
│       ├── before_after_ad.md                 # إعلان كامل قبل/بعد
│       └── copy_workshop.md                   # عشرة تمارين
│
├── docs/                                     # الموقع المرجعي (GitHub Pages)
│
├── .agents/skills/arabic-copywriting-skill/  # مسار Codex و Antigravity
│
└── .claude/skills/arabic-copywriting-skill/  # مسار Claude Code
</code></pre>

---

## 🚀 طرق التثبيت والاستخدام (Installation Guide)

تُثبَّتُ المهارةُ إما في مشروعٍ بعينه (**محلياً**)، وإما **عامةً (Global)** لتعمل في كافة المشاريع.

---

### أولاً: التثبيت بأمر واحد عبر `npx` (الطريقة الأسرع — موصى به)

```bash
npx skills add specailm5/arabic-copywriting-skill -g -y
```

ولاختيار بيئات بعينها أو التثبيت داخل مشروع محدد:

```bash
npx skills add specailm5/arabic-copywriting-skill -a claude-code -a codex
npx skills add specailm5/arabic-copywriting-skill --skill arabic-copywriting-skill -g -y
```

---

### ثانياً: التثبيت العام لبيئة Claude Code و Codex و Antigravity (يدوياً)

#### لنظام Windows (PowerShell):

```powershell
# مصدر المهارة داخل المستودع
$src = "skills\arabic-copywriting-skill"

# 1. تثبيت لبيئة Claude Code
New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.claude\skills\arabic-copywriting-skill"
Copy-Item -Recurse -Force "$src\*" "$env:USERPROFILE\.claude\skills\arabic-copywriting-skill\"

# 2. تثبيت لبيئة Codex و Agent Skills العامة
New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.agents\skills\arabic-copywriting-skill"
Copy-Item -Recurse -Force "$src\*" "$env:USERPROFILE\.agents\skills\arabic-copywriting-skill\"

# 3. تثبيت لبيئة Google Antigravity / Gemini
New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.gemini\config\skills\arabic-copywriting-skill"
Copy-Item -Recurse -Force "$src\*" "$env:USERPROFILE\.gemini\config\skills\arabic-copywriting-skill\"
```

#### لنظام macOS / Linux (Bash):

```bash
src=skills/arabic-copywriting-skill

# 1. لبيئة Claude Code
mkdir -p ~/.claude/skills/arabic-copywriting-skill
cp -r "$src/." ~/.claude/skills/arabic-copywriting-skill/

# 2. لبيئة Codex و Agent Harness
mkdir -p ~/.agents/skills/arabic-copywriting-skill
cp -r "$src/." ~/.agents/skills/arabic-copywriting-skill/

# 3. لبيئة Antigravity / Gemini
mkdir -p ~/.gemini/config/skills/arabic-copywriting-skill
cp -r "$src/." ~/.gemini/config/skills/arabic-copywriting-skill/
```

---

### ثالثاً: التثبيت المحلي داخل مشروع محدد (VS Code Workspace Harness)

```powershell
New-Item -ItemType Directory -Force -Path ".agents\skills\arabic-copywriting-skill"
Copy-Item -Recurse -Force "path\to\skills\arabic-copywriting-skill\*" ".agents\skills\arabic-copywriting-skill\"
```

---

### رابعاً: الاستخدام اليدوي (Direct System Prompt / Custom Instructions)

* افتح ملف [`skills/arabic-copywriting-skill/SKILL.md`](skills/arabic-copywriting-skill/SKILL.md) وانسخ محتواه وضعه في خانة **التعليمات المخصصة (Custom Instructions)** أو **System Prompt**.

---

## ⚡ كيف تعمل المهارة؟

### سبعة أسئلة قبل الكتابة

<table dir="rtl" align="right">
<thead>
<tr>
<th align="right">السؤال</th>
<th align="right">لماذا؟</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>ما المنتج؟</strong></td>
<td>يحدد الفائدة</td>
</tr>
<tr>
<td><strong>من الجمهور؟</strong></td>
<td>يحدد اللغة والوسيط</td>
</tr>
<tr>
<td><strong>ما المشكلة؟</strong></td>
<td>يحدد الفكرة</td>
</tr>
<tr>
<td><strong>ما الفائدة؟</strong></td>
<td>يحدد الوعد</td>
</tr>
<tr>
<td><strong>ما الدليل؟</strong></td>
<td>يحدد المصداقية</td>
</tr>
<tr>
<td><strong>ما الوسيط؟</strong></td>
<td>يحدد الطول</td>
</tr>
<tr>
<td><strong>ما الفعل؟</strong></td>
<td>يحدد CTA</td>
</tr>
</tbody>
</table>
<br clear="all">

### من الميزة إلى الفائدة

<table dir="rtl" align="right">
<thead>
<tr>
<th align="right">الميزة</th>
<th align="right">الفائدة</th>
</tr>
</thead>
<tbody>
<tr>
<td>بطارية ٥٠٠٠</td>
<td>يوم بلا شاحن</td>
</tr>
<tr>
<td>توصيل مجاني</td>
<td>لا تدفع أكثر</td>
</tr>
<tr>
<td>تصنيف تلقائي</td>
<td>تعرف أين يذهب مالك</td>
</tr>
</tbody>
</table>
<br clear="all">

### مسار العمل

<pre dir="rtl"><code>
① الجمهور والاعتراض
        ↓
② الفائدة والفكرة
        ↓
③ الوعد والدليل
        ↓
④ العنوان
        ↓
⑤ النص
        ↓
⑥ CTA
        ↓
⑦ الحملة والقياس
</code></pre>

### قبل/بعد

<table dir="rtl" align="right">
<thead>
<tr>
<th align="right">قبل</th>
<th align="right">بعد</th>
<th align="right">السبب</th>
</tr>
</thead>
<tbody>
<tr>
<td>«الحل الأمثل»</td>
<td>«فاتورتك أقل ٢٠٪»</td>
<td>فائدة</td>
</tr>
<tr>
<td>«نحن الأفضل»</td>
<td>«٣ مزودين… سعر واحد»</td>
<td>دليل</td>
</tr>
<tr>
<td>«اتصل الآن»</td>
<td>«احسب توفيرك»</td>
<td>CTA</td>
</tr>
<tr>
<td>«للجميع»</td>
<td>«صاحب فاتورة»</td>
<td>شريحة</td>
</tr>
</tbody>
</table>
<br clear="all">

---

## 📚 المراجع والاعتماد

* **«فن الإعلان: كيف تنتج وتدير إعلاناً فعالاً وحملة إعلانية ناجحة»** — أحمد فاربي — ترجمة عبد الحكم أحمد الخزامي:
  <https://archive.org/details/20201012_20201012_1531>
* **«الإعلان الفعال: منظور تطبيقي متكامل»** — علي فلاح الزعبي:
  <https://archive.org/details/20200414_20200414_1814>

> **إقرار بالفضل:** هذه المهارة صياغة تعليمية مستقلة لمبادئ الكتابين، مع نقل اقتباسات محدودة بإسنادها إلى صفحاتها. ولا يتضمّن المستودع نسخاً كاملة من الكتب، ولا يُغني عن الرجوع إلى الأصل.

---

## ⚠️ حدود المسؤولية

- المهارة **لكتابة الإعلان وتحريره**، لا لاختلاق الادعاءات أو الشهادات.
- لا تُستغل الخوف أو الضعف أو الأطفال.
- لا تُقدّم ادعاءً صحياً/قانونياً بلا مختص.
- لا تمييز على أساس جنس/لون/دين/إعاقة.
- المستخدم مسؤول عن مراجعة النص النهائي والتحقق من كل ادعاء قبل النشر.

---

## 🤝 المساهمة

نرحب بالمساهمات التي تحسّن المادة أو التحرير أو التوثيق. اقرأ [CONTRIBUTING.md](CONTRIBUTING.md) قبل فتح طلب سحب، والتزم بـ[قواعد السلوك](CODE_OF_CONDUCT.md).

## 🛡️ الأمان

إن وجدت مشكلة أمنية، فلا تفتح قضية عامة؛ راجع [SECURITY.md](SECURITY.md).

## 📄 سجل التغييرات

راجع [CHANGELOG.md](CHANGELOG.md) لمعرفة ما أُضيف في كل إصدار.

## 📬 الدعم

للأسئلة والاقتراحات: [افتح قضية](https://github.com/specailm5/arabic-copywriting-skill/issues).

---

## 📜 الترخيص (License)

هذه المهارة مفتوحة المصدر تحت رخصة [MIT](LICENSE)، ومتاحة للاستخدام الشخصي والتجاري والبحثي لدعم اللغة العربية.
