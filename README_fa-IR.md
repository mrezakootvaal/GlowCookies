<img src="https://cabas.b-cdn.net/glowcookies/glowcookies.png" data-canonical-src="https://cabas.b-cdn.net/glowcookies/glowcookies.png" width="100%" />

![Badge-glow](https://img.shields.io/badge/GlowCookies-v.3.1.8-blue?style=flat-square) ![jsDelivr hits (GitHub)](https://img.shields.io/jsdelivr/gh/hm/manucaralmo/GlowCookies?style=flat-square) [![GitHub contributors](https://img.shields.io/github/contributors/manucaralmo/GlowCookies?style=flat-square)](https://github.com/AmauriC/tarteaucitron.js/graphs/contributors) ![GitHub Repo stars](https://img.shields.io/github/stars/manucaralmo/GlowCookies?style=social)

# GlowCookies 🍪 - بنر قدرتمند رضایت کوکی در جاوا اسکریپت
بنر کوکی ساده و کامل خودکار برای هر وب سایت. مطابق با مقررات جدید اروپا با GlowCookies. کوکی های گوگل آنالیتیکس، فیس بوک پیکسل، هاتجار (و به زودی) را هر زمان که کاربر بخواهد، فقط با یک کلیک فعال و غیرفعال کنید.

[![Foo](https://cdn.glowmedia.es/upload/uploads/ed1952btn.svg)](https://manucaralmo.github.io/glow-cookies-web/)

## بنر کوکی ها
<img src="https://cdn.glowmedia.es/upload/uploads/90c82dbanner.png" data-canonical-src="https://cdn.glowmedia.es/upload/uploads/90c82dbanner.png" width="375" />

## چگونه کار می کند
فقط باید کد را نصب کنید. هنگامی که کاربر روی پذیرش کوکی ها کلیک می کند، کد رهگیری گوگل آنالیتیکس، فیس بوک پیکسل و/یا هاتجار شروع به ردیابی می کند. اگر کاربر کوکی ها را رد کند، کد رهگیری شروع به کار نخواهد کرد.

## نحوه استفاده
این کد را به تگ `<head>` یا `<body>` خود اضافه کنید.
```html
<script src="https://cdn.jsdelivr.net/gh/manucaralmo/GlowCookies@3.1.8/src/glowCookies.min.js"></script>
<script>
    glowCookies.start('en', {
        style: 1,
        analytics: 'G-FH87DE17XF',
        facebookPixel: '990955817632355',
        policyLink: 'https://link-to-your-policy.com'
    });
</script>
```

## سبک های بنر
اکنون می توانید بین این سبک های بنر موجود یکی را انتخاب کنید:
- سبک `1`, `2` یا `3`

تنظیم سبک در شی پیکربندی `glowCookies.start('en', { style: 3 })`

## زبان ها
اکنون می توانید بین این زبان های موجود یکی را انتخاب کنید:
- Afrikaans (`af`)
- Brazilian portugese (`pt_BR`)
- Bulgarian (`bg`)
- Catalan (`ca`)
- Chinese Simple (`zh`)
- Chinese Traditional (`zh_TW`)
- Danish (`da`)
- Dutch (`nl`)
- English (`en`)
- French (`fr`)
- German (`de`)
- Italian (`it`)
- Japanese (`ja`)
- Malagasy (`mg`)
- Norwegian (`no`)
- Occitan (`oc`)
- Polish (`pl`)
- Russian (`ru`)
- Slovak (`sk`)
- Spanish (`es`)
- Swedish (`sv`)
- Thai (`th`)
- Turkish (`tr`)
- Ukrainian (`uk`)
- Farsi (فارسی) (`fa`)

زبان را در پارامتر اول روش `glowCookies.start('en', { })` تنظیم کنید.

## گزینه های ردیابی
اینها پارامترهایی هستند که می توانید برای اضافه کردن کدهای رهگیری یا اسکریپت های سفارشی خود تغییر دهید.

| پارامتر               | نوع   | مقادیر                                                                                                              |
| ----------------------- | ------ | ------------------------------------------------------------------------------------------------------------------- |
| `analytics`             | رشته | نمونه: `"G-FH87DE17XF"` (کد رهگیری گوگل آنالیتیکس)                                                                 |
| `facebookPixel`         | رشته | نمونه: `"990955817632355"` (کد فیس بوک پیکسل)                                                                  |
| `HotjarTrackingCode`    | رشته | نمونه: `"990955817632355"` (کد رهگیری هاتجار)                                                                 |
| `customScript` (Inline) | رشته | نمونه: `[{ type: 'custom', position: 'body', content: 'console.log('custom script');' }]`                         |
| `customScript` (src)    | رشته | نمونه: `[{ type: 'src', position: 'head', content: 'https://www.googletagmanager.com/gtag/js?id=G-FH87DE17XF' }]` |

## پیکربندی بنر
اینها پارامترهایی هستند که می توانید برای تغییر گزینه های بنر خاص تغییر دهید

| پارامتر        | نوع    | مقادیر                                                                           |
| ---------------- | ------- | -------------------------------------------------------------------------------- |
| `policyLink`     | رشته  | نمونه: `"https://yourlink.com"` (پیوند خط مشی کوکی های شما)                     |
| `hideAfterClick` | بولین | (`true` or `false`) پیشفرض: `true` (پس از پذیرش یا رد کوکی ها، بنر را مخفی کنید) |


## شخصی سازی پنر
اکنون پارامترهای خاصی وجود دارد که می توانید آنها را تغییر دهید تا بنر خود را سفارشی کنید.

| پارامتر             | نوع   | مقادیر                                                                                                 |
| --------------------- | ------ | ------------------------------------------------------------------------------------------------------ |
| `border`              | رشته | (`"border"` or `"none"`) پیشفرض: `"border"`                                                           |
| `position`            | رشته | (`"left"` or `"right"`) پیشفرض: `"left"`                                                              |
| `bannerDescription`   | رشته | نمونه: `"We use our own and third-party cookies to personalize content and to analyze web traffic."` |
| `bannerLinkText`      | رشته | نمونه: `"Read more about cookies"`                                                                   |
| `bannerBackground`    | رشته | نمونه: `"#FAFAFA"` نمونه: `"lightblue"`                                                            |
| `bannerColor`         | رشته | نمونه: `"#000"` نمونه: `"blue"`                                                                    |
| `bannerHeading`       | رشته | نمونه: `"Use of cookies"` پیشفرض: None                                                              |
| `acceptBtnText`       | رشته | نمونه: `"Accept cookies"`                                                                            |
| `acceptBtnColor`      | رشته | نمونه: `"#000"` نمونه: `"blue"`                                                                    |
| `acceptBtnBackground` | رشته | نمونه: `"#fff"` نمونه: `"white"`                                                                   |
| `rejectBtnText`       | رشته | نمونه: `"Reject"`                                                                                    |
| `rejectBtnBackground` | رشته | نمونه: `"#000"` نمونه: `"blue"`                                                                    |
| `rejectBtnColor`      | رشته | نمونه: `"#fff"` نمونه: `"white"`                                                                   |
| `manageColor`         | رشته | نمونه: `"#fff"` نمونه: `"white"`                                                                   |
| `manageBackground`    | رشته | نمونه: `"#f2f2f2"` نمونه: `"blue"`                                                                 |
| `manageText`          | رشته | نمونه: `"Manage cookies"`                                                                            |


## بنر شخصی سازی شده کامل
```html
<script src="https://cdn.jsdelivr.net/gh/manucaralmo/GlowCookies@3.1.8/src/glowCookies.min.js"></script>
<script>
    glowCookies.start('fa', {
        style: 2,
        analytics: 'G-FH87DE17XF',
        facebookPixel: '990955817632355',
        hideAfterClick: true,
        border: 'none',
        position: 'right',
        policyLink: 'https://google.es',
        customScript: [{ type: 'custom', position: 'body', content: `console.log('my custom js');` }],
        bannerDescription: 'banner desc',
        bannerLinkText: 'banner link text',
        bannerBackground: '#000',
        bannerColor: '#fafafa',
        bannerHeading: '<h2>Cookies</h2>',
        acceptBtnText: 'accept btn text',
        acceptBtnColor: 'green',
        acceptBtnBackground: 'red',
        rejectBtnText: 'reject btn text',
        rejectBtnBackground: 'lightblue',
        rejectBtnColor: 'blue',
        manageColor: 'white',
        manageBackground: 'blue',
        manageText: 'cookies text'
    });
</script>
```

## Contribute
If you know any other language, please help translate.
- Update the `arrLang` of the `LanguageGC` class in glowCookies.js (Add an entry in this fashion.)
- Update language documentation in README.md
- Create a pull request
```
en: {
    'bannerHeading': 'We use cookies',
    'bannerDescription' : 'We use our own and third-party cookies to personalize content and to analyze web traffic.',
    'bannerLinkText' : 'Read more about cookies',
    'acceptBtnText' : 'Accept cookies',
    'rejectBtnText' : 'Reject',
    'manageText' : 'Manage cookies'
}
```
Thanks for your help! 🎉

## Next steps
- [ ] Advanced cookies management
- [ ] Cookie settings

### Request features
info@glowmedia.es
