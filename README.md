# Leon Agency - Landing Page

صفحة هبوط (Landing Page) بتصميم بسيط لشركة إبداعية، مبنية بـ **HTML + CSS** فقط (مع سكربت صغير للقائمة).

## هيكل المشروع

```
leon-agency/
├── index.html          # الصفحة الرئيسية (كل الأقسام + تعليقات توضح كل جزء)
├── README.md           # هذا الملف
├── css/
│   ├── style.css       # تنسيق الصفحة (مقسّم لأقسام مرقّمة)
│   └── all.min.css     # ملف Font Awesome (منسوخ من مجلد css في المكتبة)
├── webfonts/           # ملفات الخطوط الخاصة بـ Font Awesome (منسوخة من المكتبة)
└── images/
    └── landing.jpg     # صورة الجبال في قسم Hero
```

## شرح الكود (index.html)

| القسم | الوصف |
|-------|-------|
| `<head>` | ربط خط **Work Sans** من Google Fonts، وملف `all.min.css`، وملف `style.css` |
| Navbar | الشعار + روابط التنقل + زر القائمة للموبايل |
| Hero | عنوان "Hello There!" فوق صورة الجبال |
| Features | ثلاث ميزات بأيقونات Font Awesome |
| Services | أربع خدمات + صورة بإطار داكن |
| Portfolio | ثلاث بطاقات مشاريع + زر "Show Me More" |
| About | نص تعريفي + شكل L ملوّن |
| Contact | البريد الإلكتروني وروابط التواصل الاجتماعي |
| Footer | حقوق النشر |

## شرح التنسيق (style.css)

- **المتغيرات `:root`**: الألوان (`--teal` و `--navy`) والخط في مكان واحد لتسهيل التعديل.
- **`.container`**: يحدد عرض المحتوى ويوسّطه.
- **CSS Grid**: لتقسيم المميزات والخدمات والمشاريع.
- **`@media (max-width: 800px)`**: يحوّل الصفحة لعمود واحد ويفعّل القائمة المنسدلة.

## الخطوط والأيقونات

- **Google Fonts**: خط `Work Sans` عبر رابط `<link>` في `<head>`.
- **Font Awesome (محلي)**: أيقونات مثل `fa-gem` و `fa-pen` و `fa-twitter`. يجب وجود:
  - `css/all.min.css`
  - مجلد `webfonts/` بجانب مجلد `css` (لأن `all.min.css` يستدعي الخطوط من `../webfonts/`).

## التشغيل

افتح `index.html` في المتصفح مباشرة، أو فعّل **GitHub Pages** من إعدادات المستودع (Settings > Pages).
