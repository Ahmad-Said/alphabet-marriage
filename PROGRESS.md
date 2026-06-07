---
dir: ltr
---

# PROGRESS — Handoff & Build Strategy

> Working notes for any human or AI continuing this book. Not part of the book itself.
> The book is **«ألِف باء الزواج»**, an Arabic (فصحى) prose book derived from **50 recorded
> sessions** by **عبد الرحمن ذاكر الهاشمي**, built on the *فقه النفس* framework.

---

## 1. Locked decisions (set by the user — do not change without asking)

| Decision | Value |
|----------|-------|
| **Language / register** | Arabic, classical/formal **فصحى** (not colloquial, not bilingual) |
| **Transformation depth** | **Fully rewrite** transcripts into authored prose — *not* a cleaned transcript, *not* mere summaries |
| **Structure** | `README.md` + front matter + **أبواب** as folders; each `.md` = one فصل/topic; مغالطات-style أبواب end with **تكاليف** |
| **Ordering** | Re-ordered along the author's own delivered arc (التخلية ثم التحلية). Free to re-order; **not** bound to YouTube order |

---

## 2. The real macro-structure (corrected for all 50 sessions)

The series is **not** 10 sessions — it is **50**, in TWO halves that match the author's own labels
(confirmed from session `12-13 خطة المجالس + منهاج المجالس القادمة` and session 24, which calls
itself "المجلس الثالث من **ما لا يسعنا جهله من فقه النفس**"):

- **القسم الأول — المقدمات (s1–21):** تنبيهات/مقدمات → الجهالات والمخادعات والمغالطات (across all
  marriage stages) → خلاصات الأصول → أمانات ووصايا → مجالس الأسئلة.
- **القسم الثاني — ما لا يسعنا جهله من فقه النفس (s22–50):** الصوارف → تعريف فقه النفس → تكوّن
  النفس → الحاجات والاستعداد والإبانة → تطبيقات ومراجعات → حاجات الجنسين.

> ⚠️ **Earlier scoping error (now fixed):** the first build covered only s1–10 and mislabeled the
> مغالطات-about-the-self باب as "فقه النفس". The *real* فقه النفس is s22–50. Folder
> `02-الباب-الثاني-فقه-النفس` keeps its slug but is now **titled** "مغالطات حول النفس والآخَر".

---

## 3. Source → Chapter mapping (all 50)

Sources in [`data/raw/`](./data/raw/) as `NoteGPT_TRANSCRIPT_ألف باء الزواج NN ...`.
**Note:** session **06 is duplicated** (`...02 (1).txt` == `...02.txt`).

### القسم الأول — المقدمات
| Session(s) | Topic | → Part folder | File(s) | Status |
|---|---|---|---|---|
| 01 | المعلم/المتعلم/الجمهور | `01-الباب-الأول-مقدمات-وتنبيهات/` | `01-التعلم-يبدأ-الآن`, `02-الحكم-على-المعلم`, `03-الحكم-على-المتعلم`, `04-صوارف-التعلم-ومعيناته` | ✅ Full prose |
| 02 | المجالس وأهميتها | `01-الباب-الأول-...` | `05-المجالس-أهميتها-وما-تقدمه`, `06-تكاليف-الباب` | ✅ Full prose |
| 03 | أمشاج النفس + الحاجات | `02-الباب-الثاني-فقه-النفس/` | `01-أمشاج-النفس-الإنسانية`, `02-حاجات-النفس-الإنسانية` | ✅ Full prose |
| 04 | الآخَر | `02-الباب-الثاني-...` | `03-فقه-الآخر`, `04-تكاليف-الباب` | ✅ Full prose |
| 05–07 | مغالطات الخطبة والاختيار | `03-الباب-الثالث-الخطبة-والاختيار/` | `01-معنى-الخطبة-وأهميتها`, `02-مغالطات-الاختيار-والتفرس`, `03-الارتياح-والميل-والاستخارة`, `04-تكاليف-الباب` | ✅ Full prose |
| 08 | مغالطات عقد القران | `04-الباب-الرابع-عقد-القران/` | `01-عقد-القران-زواج-مع-وقف-التنفيذ` | 📝 Outline |
| 09 | مغالطات الزفاف وليلته | `05-الباب-الخامس-الزفاف-وليلته/` | `01-من-عقد-القران-إلى-الزفاف` | 📝 Outline |
| 10 | مغالطات ما بعد الزفاف | `06-الباب-السادس-ما-بعد-الزفاف/` | `01-شهر-العسل-والسنة-الأولى-والطلاق` | 📝 Outline |
| 11 | الأصول… ولكن! (خلاصات) | `07-الباب-السابع-الأصول/` | `01-الأصول-والاستثناءات` | 📝 Outline |
| 12 | أمانات ووصايا | `08-الباب-الثامن-أمانات-ووصايا/` | `01-أمانات-ووصايا` | 📝 Outline |
| 12-13, 13–21 | خطة المجالس + مجالس الأسئلة (إجابة أسئلة المقدمات 01–09 + خلاصات) | `09-الباب-التاسع-مجالس-الأسئلة/` | `01-منهج-الأسئلة-وخلاصاتها` | 📝 Outline |

### القسم الثاني — ما لا يسعنا جهله من فقه النفس
| Session(s) | Topic | → Part folder | File(s) | Status |
|---|---|---|---|---|
| 22–23 | صوارف ومعوقات وموانع (جـهـل، المخادعات) | `10-الباب-العاشر-الصوارف-والمعوقات/` | `01-الصوارف-والمعوقات-والمخادعات` | 📝 Outline |
| 24 | تعريف فقه النفس (الطمأنينة/السعادة) | `11-الباب-الحادي-عشر-تعريف-فقه-النفس/` | `01-تعريف-فقه-النفس` | 📝 Outline |
| 25–28 | ممّ تتكون النفس (أمشاج، الجسد والروح، الحاجات) | `11-الباب-الحادي-عشر-...` | `02-تكون-النفس-الجسد-والروح` | 📝 Outline |
| 28–32 | الحاجات + الاستعداد المادي (+ أسئلة 31–32) | `12-الباب-الثاني-عشر-الحاجات-والإبانة/` | `01-الحاجات-والاستعداد-المادي` | 📝 Outline |
| 33–34 | فقه الحاجات + الإبانة والتعبير (حاجة الحاجة) | `12-الباب-الثاني-عشر-...` | `02-فقه-الحاجات-والإبانة` | 📝 Outline |
| 35–42 | تطبيقات/خلاصات/قصص + مراجعات الجمهور 01–07 | `13-الباب-الثالث-عشر-تطبيقات-ومراجعات/` | `01-تطبيقات-ومراجعات-وقصص` | 📝 Outline |
| 43–45 | مدخل + حاجات الجنسين + حاجات الرجل | `14-الباب-الرابع-عشر-حاجات-الجنسين/` | `01-حاجات-الرجل` | 📝 Outline |
| 46–50 | حاجات المرأة 01–05 | `14-الباب-الرابع-عشر-...` | `02-حاجات-المرأة` | 📝 Outline |

Front matter (`00-مدخل-الكتاب/`): `00-عن-الكتاب`, `01-عن-المؤلف`, `02-كيف-تقرأ-هذا-الكتاب`,
`03-المنهج-والمصطلحات` — all ✅ Full prose. *(Note: `00`/`03` still say "خمسون"? verify counts say 50.)*

**Legend:** ✅ Full prose = finished chapter · 📝 Outline = headings + bullet key points marked
*«خلاصةٌ مُنظَّمة … تمهيدًا لتحريرها نثرًا كاملًا»*.

---

## 4. Reading status of sources (so the next AI knows what's been digested)

- **Fully read:** 01, 02, 03, 04 (these are the ✅ chapters).
- **Openings skimmed:** 05, 06, 07, 08, 09, 10, 11, 12-13 (roadmap), 24.
- **Filename-only (NOT yet read):** 13–23, 25–50. The 📝 outlines for these are derived from the
  very descriptive filenames + the framework already learned + the roadmap session. **Before
  writing their full prose, READ the corresponding transcript fully.**

---

## 5. Editing strategy (replicate for consistency)

1. Read the source transcript **fully** before writing (spoken Levantine, timestamps every line,
   heavy repetition/filler/live asides). Read tool caps ~25k tokens/page → page through long ones.
2. Discard session noise: timestamps, greetings, audio/tech glitches, attendee names, telegram
   logistics, off-topic banter.
3. Re-order & merge related ideas; split one session into several thematic files when warranted.
4. Rewrite in **فصحى**, preserving the author's voice/method/intent, not his literal words.
5. Keep Qur'an/hadith/sīra shawāhid + clinic anecdotes (reword anecdotes to conceal people).
6. End مغالطات-style أبواب with **تكاليف**.
7. Cross-link with relative links; add nav footers (`↩️ … · ➡️ …`).
8. Callout quotes (`>`) for the author's formulas; tables for taxonomies.

---

## 6. The book's DNA (motifs to preserve)

- **مغالطات as opposed pairs** with a balanced middle → **أمشاج**.
- **التخلية قبل التحلية**.
- Signature lines: «الحكم على الشيء فرعٌ عن تصوُّره» · «محتاجٌ ضعيفٌ فقيرٌ ناقص» · ثلاثية
  الصدق/الصبر/الرحمة · ثلاثية الصوارف **جـ‌هـ‌ل** · كافّات الهوى الخمس · مهارة **سَفَر** + تدريباتها
  العشرة · **بين قَدَرَين** · «دِينِ سُكَّرٍ خفيفٍ قليل التكليف» · «الحاجة وما فوق الحاجة» · «الطمأنينة
  لا السعادة» · «الإبانة والتعبير = حاجة الحاجة».
- Tone: واقعي، صريح، «طبيبٌ لا كوافير» — صادق غير مُداهِن، مع رحمة.

---

## 7. How to continue (priority order)

1. **Promote 📝 → ✅** by writing full prose, one فصل at a time, reading each source first.
   Suggested order: finish القسم الأول outlines (Parts 3–9), then القسم الثاني (Parts 10–14).
2. القسم الثاني is the substantive core (real فقه النفس); budget the most effort there, esp.
   **Part 12 (الحاجات/الإبانة)** and **Part 14 (حاجات الجنسين, 8 sessions)**.
3. Keep the `README.md` tables and this file's Status columns in sync as chapters are promoted.
4. Consider extracting the author's planned «نصوص القرآن والسنة المتعلقة بالزواج» (mentioned in
   the roadmap) into an appendix if those sessions appear later.

---

## 8. Current folder tree (book files only)

```
README.md
PROGRESS.md                              ← this file
00-مدخل-الكتاب/                          00..03  ✅
— القسم الأول: المقدمات —
01-الباب-الأول-مقدمات-وتنبيهات/           00 تمهيد · 01..05 ✅ · 06 تكاليف ✅      (s1–2)
02-الباب-الثاني-فقه-النفس/   [مغالطات]    00 تمهيد · 01..03 ✅ · 04 تكاليف ✅      (s3–4)
03-الباب-الثالث-الخطبة-والاختيار/         00 تمهيد · 01..03 ✅ · 04 تكاليف ✅      (s5–7)
04-الباب-الرابع-عقد-القران/               00 تمهيد · 01 📝                         (s8)
05-الباب-الخامس-الزفاف-وليلته/            00 تمهيد · 01 📝                         (s9)
06-الباب-السادس-ما-بعد-الزفاف/            00 تمهيد · 01 📝                         (s10)
07-الباب-السابع-الأصول/                   00 تمهيد · 01 📝                         (s11)
08-الباب-الثامن-أمانات-ووصايا/            00 تمهيد · 01 📝                         (s12)
09-الباب-التاسع-مجالس-الأسئلة/            00 تمهيد · 01 📝                         (s12-13,13–21)
— القسم الثاني: ما لا يسعنا جهله من فقه النفس —
10-الباب-العاشر-الصوارف-والمعوقات/        00 تمهيد · 01 📝                         (s22–23)
11-الباب-الحادي-عشر-تعريف-فقه-النفس/      00 تمهيد · 01..02 📝                     (s24–28)
12-الباب-الثاني-عشر-الحاجات-والإبانة/     00 تمهيد · 01..02 📝                     (s28–34)
13-الباب-الثالث-عشر-تطبيقات-ومراجعات/     00 تمهيد · 01 📝                         (s35–42)
14-الباب-الرابع-عشر-حاجات-الجنسين/        00 تمهيد · 01..02 📝                     (s43–50)
data/raw/                                 source transcripts (01..50; 06 duplicated)
```

_Last updated: 2026-06-07. Reworked from 10→50 sessions._
