# SomayaLuxe Theme v1.4

قالب سميّة لوكس المخصص لمنصة سلة – إصدار 1.4  
يتضمن إعدادات مخصصة ومكونات جاهزة لتخصيص مظهر المتجر بسهولة.

---

## 🧩 إعدادات الثيم

يمكنك التحكم في شكل الثيم من خلال الحقول التالية:

| المعرف | النوع | التسمية | القيمة الافتراضية |
|--------|-------|---------|--------------------|
| `topnav_is_dark` | boolean (switch) | شريط علوي داكن | true |
| `important_links` | boolean (switch) | عرض روابط مهمة في الهيدر | false |

### ✅ مثال استخدام داخل ملفات `.twig`

```twig
{% if theme.settings.get("topnav_is_dark") %}
  <div class="topnav dark">...</div>
{% else %}
  <div class="topnav light">...</div>
{% endif %}

{% if theme.settings.get("important_links") %}
  <ul class="important-links">
    <li><a href="/about">عن المتجر</a></li>
    <li><a href="/contact">اتصل بنا</a></li>
  </ul>
{% endif %}
```

---

## 🧱 المكونات المخصصة

تم تضمين المكونات التالية داخل مجلد `views/components/home/`:

| الاسم | العنوان المعروض | المسار |
|------|------------------|--------|
| enhanced-slider | صور متحركة (محسنة) | home.enhanced-slider |
| main-links | روابط سريعة | home.main-links |
| slider-products-with-header | منتجات متحركة مع خلفية | home.slider-products-with-header |
| enhanced-square-banners | صور مربعة (محسنة) | home.enhanced-square-banners |
| brands | الماركات التجارية | home.brands |
| custom-testimonials | آراء عملاء مخصصة | home.custom-testimonials |
| main-slider | سلايدر رئيسي | home.main-slider |

---

## 📝 ملاحظات

- تأكد من ربط كل مكون داخل لوحة المطور في سلة عبر إدخال المسار بدقة.
- يمكن التاجر تخصيص الإعدادات من داخل لوحة التحكم بسهولة دون الحاجة لتعديل الكود.

---

© Somaya Support 2025