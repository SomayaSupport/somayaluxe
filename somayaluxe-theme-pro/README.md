# SomayaLuxe Theme v1.4

🎨 قالب احترافي لمنصة سلة يحتوي على:
- ملف CSS مخصص لتنسيق واجهة المتجر
- إعدادات قابلة للتخصيص من لوحة التحكم
- مكون مرئي ديناميكي (قسم ترحيبي)

---

## 🧩 إعدادات الثيم

| المعرف              | النوع             | التسمية                  | القيمة الافتراضية |
|---------------------|-------------------|---------------------------|--------------------|
| topnav_is_dark      | boolean (switch)  | شريط علوي داكن           | true               |
| important_links     | boolean (switch)  | روابط مهمة في الهيدر     | false              |

```twig
{% if theme.settings.get("topnav_is_dark") %}
  <div class="topnav dark">...</div>
{% endif %}
```

---

## 🧱 المكونات

### ✅ welcome - قسم ترحيبي

| الحقل      | النوع     | التسمية       |
|------------|-----------|----------------|
| title      | string    | عنوان القسم    |
| subtitle   | textarea  | وصف القسم      |

```twig
<section>
  <h2>{{ block.settings.get('title') }}</h2>
  <p>{{ block.settings.get('subtitle') }}</p>
</section>
```

---

## 📁 الملفات

- `assets/theme.css`: تصميم مرئي عام
- `views/components/home/welcome.twig`: مكون ترحيبي مخصص
- `theme.json`: إعدادات ومكونات
- `README.md`: وثائق الاستخدام

---

© Somaya Support 2025