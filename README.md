<div align="center">

<img src="icon-192.png" width="110" alt="Kolo Arcade">

# KOLO ARCADE — ألعاب كولو

**ألعاب سريعة تعمل بلا إنترنت. العب وحدك أو مع أصدقائك على جهاز واحد.**

*Fast games that work offline. Play solo or with friends on one device.*

`الإصدار 2.0` · `Version 2.0` · `PWA` · `عربي / English` · `بلا إعلانات` · `Made in Sudan`

### [▶ العب الآن · Play now](https://ymdkwlwlw-arch.github.io/X-O-gams-ss/)

© 2026 ڪولو سآن (Red X) · جميع الحقوق محفوظة · All rights reserved

</div>

---

[العربية](#العربية) · [English](#english) · [الحقوق والترخيص](#الحقوق-والترخيص) · [Rights & License](#rights--license)

---

<a id="العربية"></a>
<div dir="rtl">

## العربية

### نبذة
**ألعاب كولو** مجموعة من عشر ألعاب خفيفة في ملف HTML واحد، تعمل على الهاتف والحاسوب دون إنترنت بعد أول فتح. لا حسابات ولا إعلانات ولا تتبّع، وبياناتك تبقى على جهازك فقط.

**الرابط المباشر:** https://ymdkwlwlw-arch.github.io/X-O-gams-ss/

### الألعاب

| اللعبة | الوصف | الأنماط |
|---|---|---|
| إكس أو | ثلاث في صف | ضد الحاسوب / لاعبان، تلميح، تراجع، وضع الرحمة |
| أربعة في صف | أسقط الأقراص واربط أربعة | ضد الحاسوب / لاعبان، تلميح، تراجع |
| ريفيرسي | اقلب أقراص خصمك واحتل الرقعة | ضد الحاسوب / لاعبان |
| النقاط والمربعات | أغلق المربعات واكسب دورًا إضافيًا | ضد الحاسوب / لاعبان |
| لعبة الذاكرة | اعثر على الأزواج بأقل حركات | فردي |
| كاسح الألغام | افتح الخانات وتجنّب الألغام | فردي |
| 2048 | ادمج الأرقام حتى 2048 | فردي (سحب أو أسهم) |
| سيمون | كرّر تسلسل الأنغام | فردي |
| اضرب الهدف | اختبر سرعة ردّ فعلك | فردي |
| مبارزة الأصابع | الأسرع في الضغط يفوز، أول من يصل إلى 5 | جهاز واحد لاثنين |

### المميزات
- **تعمل دون إنترنت:** عبر Service Worker، وقابلة للتثبيت كتطبيق.
- **اللعب مع الأصدقاء:** وضع اللاعبين على جهاز واحد بالتناوب، ومبارزة الأصابع بوجهين متقابلين.
- **ذكاء بخمسة مستويات:** سهل، متوسط، صعب، تلقائي (يتكيّف مع سلسلة انتصاراتك)، ومتعلّم.
- **الذكاء المتعلّم** (إكس أو وأربعة في صف): يتعرّف على أسلوبك ويكيّف لعبه، ويمكنك مسح ما تعلّمه في أي وقت.
- **نظام تقدّم:** خبرة XP ومستويات، ومهمة يومية، وأيام متتالية، وإنجازات.
- **مظاهر ألوان:** كلاسيك، نيون، ذهبي، نعناع (تُفتح بالمستويات).
- **ثنائية اللغة:** عربي (RTL) وإنجليزي، بتبديل فوري.
- **أصوات مولّدة داخليًا** دون ملفات صوت خارجية.
- **سريعة الاستجابة:** تناسب شاشات الهاتف وتحترم تقليل الحركة في إعدادات الجهاز.

### التثبيت واللعب
**من الرابط (الأسهل):** افتح الرابط في كروم ← القائمة ⋮ ← **تثبيت التطبيق** / Install app. وفي آيفون: سفاري ← مشاركة ← **إضافة إلى الشاشة الرئيسية**. بعد أول فتح متصل يعمل دون إنترنت.

**محليًا:** افتح `index.html` مباشرة، وللتثبيت كتطبيق قدّمه عبر `localhost`:
```bash
python -m http.server 8080
# ثم افتح http://localhost:8080
```

### سجل الإصدارات

**الإصدار 2.0** (2026)
- حذف الثعبان وحجر ورقة مقص.
- إضافة أربع ألعاب: ريفيرسي، النقاط والمربعات، كاسح الألغام، مبارزة الأصابع.
- واجهة القائمة بعمودين، وإنجازات جديدة.
- قسم «حول التطبيق».
- أيقونة جديدة، وتحسين العمل دون إنترنت.
- الذكاء المتعلّم يبقى في إكس أو وأربعة في صف.

**الإصدار 1.0**
- إكس أو، أربعة في صف، الذاكرة، حجر ورقة مقص، الثعبان، 2048، سيمون، اضرب الهدف.
- نظام الخبرة والمستويات والمهمة اليومية والمظاهر.

### هيكل المشروع
```
├── index.html            التطبيق كاملًا (واجهة + ألعاب + ذكاء)
├── sw.js                 Service Worker للعمل دون إنترنت
├── manifest.webmanifest  بيانات التثبيت
├── icon-192.png
├── icon-512.png
├── LICENSE               الحقوق والترخيص
└── README.md
```
**عند تحديث الملفات** غيّر رقم الذاكرة في `sw.js` (مثل `kolo-v3` إلى `kolo-v4`) كي يحمّل المتصفح النسخة الجديدة.

### الخصوصية والبيانات
تُحفظ الإعدادات والنتائج وتعلّم الذكاء في `localStorage` على جهازك فقط، ولا يُرسل شيء إلى أي خادم، ولا تُجمع أي بيانات. مسح بيانات المتصفح يمسحها.

### حدود معروفة
- لا يوجد لعب بين جهازين عبر الشبكة، فالتناوب على جهاز واحد فقط.
- الذكاء المتعلّم يتاح في إكس أو وأربعة في صف فقط.
- مهمة اليوم تُحسب بتاريخ الجهاز.

### حول المشروع
> لا مؤسسة وراء هذا العمل ولا فريق؛ يدان اثنتان وسهر ليالٍ. إن وجدتَ فيه خيرًا فأعِده إلى صاحبه، وإن وجدتَ خللًا فدلّني عليه، فما زلتُ أتعلّم.

**المطوّر:** ڪولو سآن (Red X) · صنع في السودان
**الحساب:** [@ymdkwlwlw-arch](https://github.com/ymdkwlwlw-arch)

*اللهم بارك له في علمه ووقته، واجعل عمله خالصًا لوجهك الكريم.*

### الإبلاغ عن مشكلة أو اقتراح
افتح [Issues](https://github.com/ymdkwlwlw-arch/X-O-gams-ss/issues) واذكر: نوع الجهاز والمتصفح، واللعبة، وخطوات تكرار المشكلة، ولقطة شاشة إن أمكن. كل ملاحظة موضع شكر.

<a id="الحقوق-والترخيص"></a>
### الحقوق والترخيص

**© 2026 ڪولو سآن (Red X). جميع الحقوق محفوظة.**

هذا العمل، ويشمل الكود والتصميم والأيقونة والنصوص والأسماء، ملك لمطوّره. الكود ظاهر للاطلاع والتعلّم فقط، وليس مفتوح المصدر.

**مسموح:**
- اللعب واستخدام التطبيق للاستعمال الشخصي وغير التجاري، ومشاركة رابطه.
- قراءة الكود للتعلّم.

**غير مسموح دون إذن كتابي مسبق من المطوّر:**
- نسخ الكود أو أي جزء منه أو إعادة نشره.
- تعديله أو البناء عليه أو نشر نسخة مشتقة.
- بيعه أو إعادة تغليفه كتطبيق أو نشره في متجر تحت اسم آخر.
- إزالة اسم المطوّر أو قسم «حول التطبيق» أو إشعار الحقوق.

لطلب إذن أو للاستفسار افتح [Issue](https://github.com/ymdkwlwlw-arch/X-O-gams-ss/issues) في المستودع. والنص الكامل في ملف [LICENSE](LICENSE).

> ملاحظة: بحكم شروط استخدام GitHub، يحق لمن يرى المستودع العام أن يعمل له Fork داخل المنصة لغرض الاطلاع، وهذا لا يمنحه حق إعادة النشر أو الاستخدام خارجها.

</div>

---

<a id="english"></a>

## English

### About
**Kolo Arcade** is a collection of ten lightweight games in a single HTML file. It runs on phones and desktops and works offline after the first load. No accounts, no ads, no tracking: your data never leaves your device.

**Live:** https://ymdkwlwlw-arch.github.io/X-O-gams-ss/

### Games

| Game | Description | Modes |
|---|---|---|
| Tic-Tac-Toe | Three in a row | Vs computer / two players, hint, undo, mercy mode |
| Connect Four | Drop discs, link four | Vs computer / two players, hint, undo |
| Reversi | Flip your rival's discs and own the board | Vs computer / two players |
| Dots & Boxes | Close boxes and earn extra turns | Vs computer / two players |
| Memory | Match pairs in few moves | Solo |
| Minesweeper | Open cells, avoid the mines | Solo |
| 2048 | Merge tiles up to 2048 | Solo (swipe or arrow keys) |
| Simon | Repeat the tone sequence | Solo |
| Aim Trainer | Test your reaction speed | Solo |
| Finger Duel | Fastest tap wins, first to 5 | One device, two players |

### Features
- **Offline-first** via a Service Worker, installable as an app.
- **Play with friends** on one device by taking turns; Finger Duel is built for two players facing each other.
- **Five AI levels:** Easy, Medium, Hard, Auto (adapts to your win streak), and Learner.
- **Learning AI** (Tic-Tac-Toe, Connect Four): adapts to your play style; you can reset what it learned any time.
- **Progression:** XP and levels, a daily mission, day streaks, achievements.
- **Color themes:** Classic, Neon, Gold, Mint (unlocked by level).
- **Bilingual:** Arabic (RTL) and English with instant switching.
- **Procedurally generated sounds**, no external audio files.
- **Responsive**, mobile-first, and respects reduced-motion settings.

### Install & play
**From the link (easiest):** open it in Chrome → menu ⋮ → **Install app**. On iPhone: Safari → Share → **Add to Home Screen**. After the first online load it works offline.

**Locally:** open `index.html` directly, or serve it on `localhost` to install it:
```bash
python -m http.server 8080
# then open http://localhost:8080
```

### Changelog

**Version 2.0** (2026)
- Removed Snake and Rock Paper Scissors.
- Added four games: Reversi, Dots & Boxes, Minesweeper, Finger Duel.
- Two-column game menu and new achievements.
- New "About" section.
- New icon and improved offline support.
- The learning AI remains in Tic-Tac-Toe and Connect Four.

**Version 1.0**
- Tic-Tac-Toe, Connect Four, Memory, Rock Paper Scissors, Snake, 2048, Simon, Aim Trainer.
- XP, levels, daily mission and themes.

### Project structure
```
├── index.html            the whole app (UI + games + AI)
├── sw.js                 Service Worker for offline use
├── manifest.webmanifest  install metadata
├── icon-192.png
├── icon-512.png
├── LICENSE               rights and license
└── README.md
```
**When you update the files**, bump the cache name in `sw.js` (e.g. `kolo-v3` to `kolo-v4`) so browsers fetch the new version.

### Privacy & data
Settings, scores and AI learning are stored in `localStorage` on your device only. Nothing is sent to any server and no data is collected. Clearing browser data erases them.

### Known limits
- No networked play between two devices; friends take turns on one device.
- The learning AI exists only in Tic-Tac-Toe and Connect Four.
- The daily mission uses the device's date.

### About the project
> No company stands behind this work and no team: just two hands and sleepless nights. If you find good in it, return it to its owner; if you find a flaw, point it out to me, for I am still learning.

**Developer:** ڪولو سآن (Red X) · Made in Sudan
**Account:** [@ymdkwlwlw-arch](https://github.com/ymdkwlwlw-arch)

*May Allah bless his knowledge and time, and make his work sincere.*

### Reporting issues or suggestions
Open an [Issue](https://github.com/ymdkwlwlw-arch/X-O-gams-ss/issues) and include: device and browser, the game, steps to reproduce, and a screenshot if possible. Every report is appreciated.

### Rights & License

**© 2026 ڪولو سآن (Red X). All rights reserved.**

This work, including its code, design, icon, text and names, belongs to its developer. The source is visible for viewing and learning only; it is not open source.

**Allowed:**
- Playing and using the app for personal, non-commercial use, and sharing its link.
- Reading the code to learn.

**Not allowed without prior written permission from the developer:**
- Copying the code or any part of it, or republishing it.
- Modifying it, building on it, or publishing a derivative.
- Selling it, repackaging it as an app, or publishing it to a store under another name.
- Removing the developer's name, the "About" section, or the copyright notice.

To request permission or ask a question, open an [Issue](https://github.com/ymdkwlwlw-arch/X-O-gams-ss/issues) in this repository. The full text is in the [LICENSE](LICENSE) file.

> Note: under GitHub's Terms of Service, anyone viewing a public repository may fork it within the platform for viewing purposes. This does not grant any right to republish or use it outside the platform.

---

<div align="center">

صنع في السودان · Made in Sudan · © 2026 ڪولو سآن (Red X)

</div>
