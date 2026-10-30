# NB-DOC-001 | استاندارد مستندسازی و کتاب زنده نیک‌وی
# NIKWAY Documentation & Living Book Standard

| Field | Value |
|---|---|
| Document ID | NB-DOC-001 |
| Version | 0.1.0 |
| Status | Proposed — not yet approved |
| Date | 2026-10-31 |
| Exact event time | Not recorded |
| Time zone | Asia/Tehran |
| Scope | NIKWAY documentation, narrative, decisions, evidence, publishing |
| Languages | Persian and English |
| Repository | alikhosravi90/Nikway |

> **دامنه:** این سند قواعد ثبت مسیر واقعی نیک‌وی را تعیین می‌کند؛ نه معماری فنی یا مجوز اجرای پروژه را. / This document governs the documentation of NIKWAY's actual journey, not technical architecture or execution authorization.

## ۱. هدف | Purpose
مستندسازی شناخت، تصمیم، اقدام، نتیجه و تکامل نیک‌وی به‌صورتی که تاریخچه معتبر باقی بماند و بتوان از آن کتاب، Handbook، Playbook، گزارش و محتوای دوزبانه منتشر کرد.

Document NIKWAY's understanding, decisions, actions, outcomes, and evolution with traceable history and reusable bilingual publishing sources.

## ۲. اصول الزام‌آور | Principles
1. **مرجع مشخص / Canonical source:** هر مفهوم، تصمیم و رویداد مرجع یکتا یا شناسه ارجاع‌پذیر دارد.
2. **شواهد / Evidence:** مشاهده، تفسیر، فرضیه، پیشنهاد، تصمیم و نتیجه تأییدشده از هم جدا هستند.
3. **زمان / Time:** زمان وقوع، ثبت، بازبینی و انتشار یکسان فرض نمی‌شوند.
4. **تاریخچه / History:** اصلاحات با ردپا ثبت می‌شوند؛ روایت جدید نباید دانسته‌های امروز را به گذشته نسبت دهد.
5. **توسعه تدریجی / Progressive elaboration:** اسناد و مدل‌ها با کسب شناخت تکامل می‌یابند.
6. **دوزبانگی / Bilingual parity:** متن فارسی و انگلیسی شناسه محتوایی مشترک و وضعیت همگام‌سازی دارند.
7. **بازاستفاده / Reuse:** Journal، Book، Playbook و Handbook به منابع یکدیگر ارجاع می‌دهند، نه اینکه نسخه‌های متناقض بسازند.
8. **امنیت و حق نشر / Safety & rights:** اطلاعات محرمانه، اسرار، داده مشتری و محتوای فاقد مجوز بازنشر در مخزن عمومی منتشر نمی‌شوند.
9. **استقلال ابزار / Tool independence:** Markdown و Git منبع اصلی‌اند؛ ابزار چاپ و سایت قابل‌تعویض است.
10. **مرز اختیار / Authority:** ثبت سند یا موفقیت آزمون به معنی مجوز Merge، Deploy یا اجرای محصول نیست.

## ۳. انواع اسناد | Document Types
| Code | فارسی | English |
|---|---|---|
| NB-DOC | استاندارد | Standard |
| NB-EVT | رویداد | Journal Event |
| NB-CON | مفهوم | Concept |
| NB-MOD | مدل | Model |
| NB-ADR | تصمیم | Decision Record |
| NB-EVD | شاهد | Evidence Record |
| NB-RPT | گزارش | Report |
| NB-PLB | راهنمای عملی | Playbook |
| NB-CH | فصل کتاب | Book Chapter |

شناسه‌ها پس از تخصیص بازاستفاده نمی‌شوند. / Identifiers are never reassigned.

## ۴. فراداده حداقلی | Minimum Metadata
هر سند: شناسه، عنوان FA/EN، نسخه، وضعیت، مالک/نویسنده، تاریخ ثبت، دامنه، منابع، روابط و تاریخچه تغییرات.

زمان دقیق باید به صورت ISO 8601 همراه با offset ذخیره شود؛ UTC می‌تواند مرجع محاسباتی باشد و Asia/Tehran برای نمایش استفاده شود. زمان نامعلوم **unknown** باقی می‌ماند. Commit timestamp جایگزین زمان واقعی رویداد نیست.

## ۵. دفتر وقایع | Journal
هر رویداد باید تا حد امکان ثبت کند:
- شناسه، زمان رخداد و زمان ثبت
- ناظر، موضوع، کانتکست و هدف
- پرسش/محرک و مشاهده
- شواهد و منبع
- تفسیر و عدم‌قطعیت
- نتیجه و پیوند به تصمیم/مدل/Commit

تصحیح یک رویداد تاریخی با ثبت اصلاحیه و ارجاع به نسخه قبلی انجام می‌شود. / Corrections remain traceable.

## ۶. ثبت تصمیم | Decision Record
قالب تصمیم: **Context → Problem/Need → Options → Criteria → Decision → Rationale → Consequences → Evidence → Authority → Status**.

وضعیت‌ها: Proposed, Accepted, Rejected, Superseded, Withdrawn. هیچ تصمیم Proposed را نباید مصوب معرفی کرد.

## ۷. ساختار روایت کتاب | Narrative Chapter
هر فصل متناسب با موضوع شامل: پرسش آغازین، زمینه تاریخی، روایت کشف، مفاهیم، منابع، مدل/تصویر، مثال، گزینه‌ها، تصمیم‌ها، درس‌آموخته، راهنمای کاربرد و تاریخچه بازنگری است.

**Journal** ثبت آنچه واقعاً رخ داد است؛ **Book** روایت تدوین‌شده؛ **Playbook** روش تکرارپذیر انجام کار؛ **Handbook** راهنمای مرجع. این چهار خروجی با یکدیگر ارتباط دارند اما یکسان نیستند.

## ۸. دوزبانگی | Bilingual Workflow
برای هر محتوای منتشرشدنی: `content_id`, `language`, `content_version`, `source_revision`, `translation_status`.

وضعیت ترجمه: Not Started / Draft / In Review / Synchronized. تغییر ادعا یا تصمیم در ترجمه بدون بازبینی محتوایی مجاز نیست.

## ۹. نسخه‌بندی | Versioning
نسخه اسناد: `MAJOR.MINOR.PATCH`.
- MAJOR: تغییر ناسازگار در معنا یا قرارداد
- MINOR: توسعه سازگار
- PATCH: اصلاح نگارشی یا فنی بدون تغییر معنا

نسخه کتاب، سند، مدل و نرم‌افزار مستقل‌اند. هر انتشار باید به Git Tag، Commit SHA، تاریخ، فهرست تغییرات و وضعیت بازبینی متصل شود.

## ۱۰. منابع و شواهد | Sources & Evidence
برای منابع: عنوان، پدیدآور/ناشر، نسخه، سال، URL/شناسه، تاریخ دسترسی و محدودیت استفاده ثبت شود. منابع اولیه، ثانویه و داخلی تفکیک شوند. نقل‌قول مستقیم، تفسیر و بازنویسی برچسب روشن داشته باشند.

## ۱۱. گردش کار | Workflow
```text
Question / Event
  → Journal + Evidence
  → Concept / Model
  → Analysis + Decision
  → Book / Playbook / Handbook
  → Review
  → Versioned Release
  → Feedback
```
این جریان تکرارشونده است و ترتیب آن در موارد خاص قابل تغییر است.

## ۱۲. Local-first و انتشار | Local-first & Publishing
Git محلی برای نگارش و ثبت نسخه‌ها؛ GitHub برای همگام‌سازی و همکاری. Markdown منبع اصلی است. Quarto گزینه اولیه انتشار HTML/PDF/EPUB است و تا آزمون موفق فارسی RTL، صفحه‌آرایی و بازتولید خروجی به‌عنوان ابزار نهایی تأیید نمی‌شود.

## ۱۳. کنترل کیفیت | Acceptance Checklist
- [ ] شناسه و نسخه معتبر
- [ ] منشأ و وضعیت ادعاها روشن
- [ ] تاریخ‌ها بدون حدس ثبت شده
- [ ] لینک‌ها و ارجاعات قابل‌بررسی
- [ ] اطلاعات حساس حذف یا محافظت شده
- [ ] ترجمه و معنی بررسی شده
- [ ] تاریخچه و مرجع Commit مشخص
- [ ] کیفیت RTL، تصاویر و خروجی چاپی بررسی شده (در صورت انتشار)
- [ ] تأیید مالک/بازبین ثبت شده

## ۱۴. حاکمیت و وضعیت | Governance
این سند **پیش‌نویس پیشنهادی** است. مخزن جدید، روایت مسیر فعلی نیک‌وی را ثبت می‌کند. پروژه‌ها و دارایی‌های پیشین بدون مجوز مستقل حذف، ادغام یا بازنویسی نمی‌شوند. هیچ توقف عملیاتی از ثبت این سند استنتاج نمی‌شود.

**Next:** بازبینی مالک، تصمیم تأیید/اصلاح، سپس ایجاد نخستین Journal و فصل دوزبانه.
