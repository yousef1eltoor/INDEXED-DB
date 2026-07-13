```markdown
<div align="center">

# 🗄️ DB Vault — مدير قواعد البيانات
### IndexedDB File Explorer & Manager

[![Offline Ready](https://img.shields.io/badge/Works-Offline-brightgreen?style=flat-square)]()
[![Zero Dependencies](https://img.shields.io/badge/Zero-Dependencies-blue?style=flat-square)]()
[![Single File](https://img.shields.io/badge/Single-File-orange?style=flat-square)]()
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)]()

**استكشف، عاين، حمّل، واحذف كل ملف مخزّن في IndexedDB مباشرة من المتصفح**
**Explore, preview, download, and delete every file stored in IndexedDB — directly from your browser**

</div>

---

## 🧑‍💻 المطور | Developer

<div align="center">

<table>
<tr>
<td width="50%" align="center">

🇪🇬

### Y M.Rashad

مطور أدوات ويب متقدم
متخصص في بناء تطبيقات تعمل بالكامل في المتصفح
محترف في استخدام نماذج الذكاء الاصطناعي لتسريع وتحسين عملية التطوير

</td>
<td width="50%" align="center">

🇬🇧

### Y M.Rashad

Advanced Web Tools Developer
Specialized in building browser-native applications
Proficient in leveraging AI models to accelerate and enhance development

</td>
</tr>
</table>

</div>

---

## ✨ الميزات الرئيسية | Key Features

<table>
<tr>
<td width="50%">

### 🇪🇬

- 🔍 **فحص تلقائي شامل** — يكتشف كل قواعد البيانات والمخازن والملفات المخزنة
- 👁️ **معاينة ذكية** — صور، فيديو، صوت، نص، PDF، وعرض Hex للملفات الثنائية
- 📥 **تحميل مباشر** — حمّل أي ملف من IndexedDB إلى جهازك
- 🗑️ **حذف دقيق** — احذف ملفاً واحداً أو قاعدة بيانات كاملة
- ✏️ **إعادة تسمية القواعد** — مع الحفاظ على كامل البيانات والهيكل
- 🎵 **مشغل موسيقى مدمج** — شريط تحكم مستقل بتقدم وصوت
- 🔎 **بحث فوري** — بالاسم أو الامتداد مع عرض عدد النتائج لحظياً
- 📂 **تبويبات الامتدادات** — داخل كل قاعدة مصنّف حسب الامتداد مع العداد
- 🌍 **ثنائي اللغة** — عربي كامل (RTL) وإنجليزي كامل (LTR)
- 🎨 **6 سمات** — داكن، فاتح، هاكر، محيط، غروب، وردي
- 🌧️ **مطر المصفوفة** — تأثير Matrix Rain مع تحكم بالشدة
- 📊 **لوحة تحكم** — إحصائيات شاملة وشريط التخزين المستخدم
- 📱 **متجاوب** — يعمل بسلاسة على الموبايل والديسكتوب
- ⚡ **صفر تبعيات** — ملف HTML واحد فقط
- 🚫 **بدون إنترنت** — يعمل بالكامل أوفلاين

</td>
<td width="50%">

### 🇬🇧

- 🔍 **Automatic Full Scan** — Detects all databases, stores, and stored files
- 👁️ **Smart Preview** — Images, video, audio, text, PDF, and Hex view for binary files
- 📥 **Direct Download** — Download any file from IndexedDB to your device
- 🗑️ **Precise Deletion** — Delete a single file or an entire database
- ✏️ **Database Renaming** — While preserving all data and structure
- 🎵 **Built-in Music Player** — Standalone control bar with progress and volume
- 🔎 **Instant Search** — By name or extension with live result count
- 📂 **Extension Tabs** — Inside each DB, sorted by extension with counters
- 🌍 **Bilingual** — Full Arabic (RTL) and Full English (LTR)
- 🎨 **6 Themes** — Dark, Light, Hacker, Ocean, Sunset, Rose
- 🌧️ **Matrix Rain** — Matrix Rain effect with intensity control
- 📊 **Dashboard** — Comprehensive stats and storage usage bar
- 📱 **Responsive** — Smooth on mobile and desktop
- ⚡ **Zero Dependencies** — Single HTML file only
- 🚫 **No Internet** — Works completely offline

</td>
</tr>
</table>

---

## 🚀 التثبيت والاستخدام | Installation & Usage

<table>
<tr>
<td>

### 🇪🇬

1. حمّل ملف `index.html`
2. افتحه في أي متصفح حديث
3. انتهى! 🎉

**لا حاجة لخادم، لا حاجة للإنترنت.**

```bash
open index.html
```

</td>
<td>

### 🇬🇧

1. Download the `index.html` file
2. Open it in any modern browser
3. That's it! 🎉

**No server needed, no internet needed.**

```bash
open index.html
```

</td>
</tr>
</table>

---

## 🏗️ كيف يعمل | How It Works

<table>
<tr>
<td>

### 🇪🇬

يعمل التطبيق على أربع مراحل:

1. **الفحص** — يستدعي `indexedDB.databases()` للحصول على قائمة بكل القواعد وإصداراتها
2. **الفتح** — يفتح كل قاعدة بإصدارها الصحيح لمنع `onupgradeneeded` الذي قد يسبب التعليق
3. **الاستخراج** — يقرأ كل مخزن سجلًا سجلًا ويبحث عن Blob أو ArrayBuffer في خصائص السجل
4. **التصنيف** — يحدد نوع الملف بناءً على الامتداد أو MIME type ويعرضه وفقًا لذلك

التطبيق لا يعتمد على هيكل بيانات محدد — يبحث في **كل** خصائص السجل عن أي بيانات ثنائية، مما يجعله متوافقاً مع أي تطبيق يستخدم IndexedDB.

</td>
<td>

### 🇬🇧

The app works in four stages:

1. **Scanning** — Calls `indexedDB.databases()` to list all databases and their versions
2. **Opening** — Opens each DB with its exact version to prevent `onupgradeneeded` from causing hangs
3. **Extraction** — Reads each store record-by-record, searching for Blob or ArrayBuffer in record properties
4. **Classification** — Determines file type by extension or MIME type and displays accordingly

The app doesn't rely on any specific data structure — it searches **all** properties of a record for binary data, making it compatible with any IndexedDB-based application.

</td>
</tr>
</table>

---

## 🎨 السمات | Themes

<div align="center">

| 🌑 Dark | ☀️ Light | 💚 Hacker | 🌊 Ocean | 🌅 Sunset | 🌸 Rose |
|:---:|:---:|:---:|:---:|:---:|:---:|
| أسود + أخضر زاهي | أبيض + أخضر داكن | أسود + أخضر نيون | أزرق داكن + سماوي | أحمر داكن + برتقالي | بنفسجي + وردي |

</div>

---

## 📁 بنية المشروع | Project Structure

```
db-vault/
│
├── index.html    ← الملف الوحيد المطلوب | The only file you need
├── README.md     ← التوثيق | Documentation
└── LICENSE       ← رخصة MIT | MIT License
```

> كل شيء — HTML, CSS, JavaScript — في ملف واحد. لا تبعيات، لا CDN.
> Everything — HTML, CSS, JavaScript — in a single file. No dependencies, no CDN.

---

## 🛠️ التقنيات | Tech Stack

| HTML5 | CSS3 (Custom Properties) | Vanilla JavaScript | IndexedDB API | Canvas API | Web Storage | File & Blob APIs |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|

---

## 🗺️ خريطة الصفحات | Page Map

<div align="center">

```
┌──────────────────────────────────────────────┐
│              🏠 Dashboard                     │
│       Stats · Quick Access · Recent Files     │
└──┬──────────┬──────────┬──────────┬──────────┘
   │          │          │          │
┌──▼──┐  ┌───▼───┐  ┌──▼───┐  ┌──▼───┐
│ 📁  │  │ 🎵    │  │ 🎬   │  │ 🖼️   │
│ All │  │ Music │  │Video │  │Images│
│Files│  │       │  │      │  │      │
└──┬──┘  └───────┘  └──────┘  └──────┘
   │
┌──▼──────────────────────┐
│ 🗄️ Databases            │
└──┬──────────────────────┘
   │ Open DB
┌──▼──────────────────────┐
│ 📋 DB Details           │
│  ┌────┬────┬────┬────┐  │
│  │All │jpg │mp3 │txt │  │
│  │ 12 │  3 │  5 │  2 │  │
│  └────┴────┴────┴────┘  │
│  ┌──────────────────┐   │
│  │   File List      │   │
│  └──────────────────┘   │
└─────────────────────────┘
                ┌──────────────────┐
                │ ⚙️ Settings      │
                │ Lang·Theme·FX   │
                └──────────────────┘
```

</div>

---

## 🧪 الاختبار | Testing

<table>
<tr>
<td>

### 🇪🇬

افتح console المتصفح والصق:

```javascript
const req = indexedDB.open('TestDB', 1);
req.onupgradeneeded = e => {
  const db = e.target.result;
  db.createObjectStore('images');
  db.createObjectStore('documents');

  fetch('https://picsum.photos/800/600')
    .then(r => r.blob())
    .then(b => {
      const tx = db.transaction('images','readwrite');
      tx.objectStore('images').put({
        name: 'photo.jpg', type: 'image/jpeg', file: b
      }, 'img-1');
    });

  const tx2 = db.transaction('documents','readwrite');
  tx2.objectStore('documents').put({
    name: 'notes.txt',
    content: new Blob(['مرحباً من DB Vault!'], {type:'text/plain'})
  }, 'doc-1');
};
```

ثم افتح DB Vault — ستظهر القاعدة مع كل الملفات.

</td>
<td>

### 🇬🇧

Open browser console and paste:

```javascript
const req = indexedDB.open('TestDB', 1);
req.onupgradeneeded = e => {
  const db = e.target.result;
  db.createObjectStore('images');
  db.createObjectStore('documents');

  fetch('https://picsum.photos/800/600')
    .then(r => r.blob())
    .then(b => {
      const tx = db.transaction('images','readwrite');
      tx.objectStore('images').put({
        name: 'photo.jpg', type: 'image/jpeg', file: b
      }, 'img-1');
    });

  const tx2 = db.transaction('documents','readwrite');
  tx2.objectStore('documents').put({
    name: 'notes.txt',
    content: new Blob(['Hello from DB Vault!'], {type:'text/plain'})
  }, 'doc-1');
};
```

Then open DB Vault — the database will appear with all files.

</td>
</tr>
</table>

---

## 🔒 الخصوصية | Privacy

<table>
<tr>
<td>

- لا يرسل أي بيانات لأي خادم
- يعمل محلياً بالكامل داخل المتصفح
- لا يكتب أي بيانات في IndexedDB — يقرأ فقط
- localStorage يحتفظ بالسمة واللغة فقط
- الكود مفتوح بالكامل للمراجعة

</td>
<td>

- Sends zero data to any server
- Runs entirely locally in the browser
- Doesn't write to IndexedDB — reads only
- localStorage holds theme and language only
- Fully open-source code for review

</td>
</tr>
</table>

---

## 🌐 التوافق | Compatibility

| Chrome 80+ | Firefox 78+ | Edge 80+ | Safari 14+ | Opera 67+ |
|:---:|:---:|:---:|:---:|:---:|
| ✅ | ✅ | ✅ | ✅ | ✅ |

---

## 📊 المقاييس | Metrics

| المقياس | Metric | القيمة | Value |
|---|---|---|---|
| حجم الملف | File Size | ~45 KB | ~45 KB |
| الأسطر | Lines | ~1,800 | ~1,800 |
| التبعيات | Dependencies | 0 | 0 |
| طلبات الشبكة | Network Requests | 0 | 0 |

---

## 🤝 المساهمة | Contributing

<table>
<tr>
<td>

1. Fork المستودع
2. أنشئ فرعاً: `git checkout -b feature/name`
3. Commit: `git commit -m 'Add feature'`
4. Push: `git push origin feature/name`
5. أرسل Pull Request

**أفكار مقترحة:**
- تصدير قاعدة بيانات كاملة كـ JSON
- عرض هيكل الفهارس
- دعم Web Workers للفحص في الخلفية
- وضع داكن تلقائي حسب النظام

</td>
<td>

1. Fork the repo
2. Create a branch: `git checkout -b feature/name`
3. Commit: `git commit -m 'Add feature'`
4. Push: `git push origin feature/name`
5. Submit a Pull Request

**Suggested ideas:**
- Full database export as JSON
- Index structure viewer
- Web Workers for background scanning
- Auto dark mode based on OS

</td>
</tr>
</table>

---

## ⚖️ الرخصة | License

مرخص تحت **MIT** — استخدام، تعديل، وتوزيع بحرية مع الاحتفاظ بنص الرخصة.
Licensed under **MIT** — use, modify, and distribute freely with the license text included.

---

<div align="center">

<br>

**طوّر بواسطة | Developed by**

## Y M.Rashad

🇪🇬 مطور أدوات ويب متقدم · محترف في استخدام نماذج AI
🇬🇧 Advanced Web Tools Developer · Proficient in AI Models

<br>

<sub>صُنع بـ ❤️ بدون أي تبعيات — ملف واحد يعمل أوفلاين</sub>
<sub>Made with ❤️ zero dependencies — a single file that works offline</sub>

</div>
```
