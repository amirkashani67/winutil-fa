# Automation و Presetها

WinUtil امکان اجرای تنظیمات بدون انتخاب دستی را فراهم می‌کند.

## Presetهای رسمی فعلی

### Standard

برای کاربر معمولی و نصب تازه Windows، مجموعه‌ای متعادل از Tweaks را اعمال می‌کند.

### Minimal

برای کسانی که می‌خواهند کمترین تغییرات ممکن انجام شود.

### Advanced

برای کاربران حرفه‌ای که کنترل بیشتری روی Windows می‌خواهند.

نمونه اجرای Standard:

```powershell
& ([ScriptBlock]::Create((irm https://christitus.com/win))) -Preset Standard
```

## چرا Preset مهم است؟

Preset چند انتخاب را یکجا اجرا می‌کند. بنابراین قبل از اجرای آن باید بدانید چه گزینه‌هایی داخل آن هستند. در نسخه فعلی، Presetها در `config/preset.json` تعریف می‌شوند.

## توسعه و ساختار پروژه

ساختار مهم پروژه اصلی شامل این بخش‌هاست:

- `config/applications.json`: فهرست برنامه‌ها
- `config/tweaks.json`: تعریف Tweaks
- `config/feature.json`: Windows Features
- `config/preset.json`: Presetها
- `config/dns.json`: گزینه‌های DNS
- `functions/public`: توابع عمومی
- `functions/private`: توابع داخلی
- `scripts`: اسکریپت‌های کمکی
- `xaml`: رابط کاربری
- `Compile.ps1`: فرآیند Build

## Export/Import

در نسخه‌های جدید، تنظیمات Exportشده به شکل JSON تخت ذخیره می‌شوند. اگر هنگام Import با خطای `Unknown selection key '<key>'` روبه‌رو شدید، احتمال دارد فایل تنظیمات مربوط به نسخه‌ای قدیمی باشد و کلید موردنظر دیگر در WinUtil وجود نداشته باشد.

## اصل مهم Automation

Automation را روی چند سیستم فقط پس از تست روی یک سیستم آزمایشی اجرا کنید. تغییرات سیستم‌عامل ممکن است بین Buildهای مختلف Windows متفاوت باشند.
