# راهنمای جامع WinUtil

## 1. پیش‌نیازها

طبق مستندات فعلی پروژه، WinUtil برای Windows 11 طراحی شده است و برای اجرای کامل به PowerShell 5.1 یا بالاتر، دسترسی Administrator، اتصال اینترنت برای اجرای اولیه و دریافت برنامه‌ها، و .NET Framework 4.5 یا بالاتر نیاز دارد.

WinUtil یک برنامه نصب‌شده دائمی نیست؛ اسکریپت در زمان اجرا دریافت و در حافظه اجرا می‌شود.

## 2. اجرای WinUtil

PowerShell یا Windows Terminal را با Run as Administrator باز کنید و:

```powershell
irm https://christitus.com/win | iex
```

نسخه توسعه:

```powershell
irm https://christitus.com/windev | iex
```

اگر Execution Policy مانع اجرا شد، راهکار موقت برای همان Process:

```powershell
Set-ExecutionPolicy Unrestricted -Scope Process -Force
```

## 3. تب Applications

در این بخش برنامه‌ها با WinGet/Chocolatey مدیریت می‌شوند.

- Install: نصب برنامه‌های انتخاب‌شده
- Upgrade: به‌روزرسانی برنامه‌های انتخاب‌شده
- Uninstall: حذف برنامه‌های انتخاب‌شده
- Upgrade All: تلاش برای به‌روزرسانی همه برنامه‌های قابل مدیریت
- Search: جست‌وجوی بسته‌ها
- Installed: مشاهده برنامه‌های نصب‌شده

نکته: قبل از حذف برنامه‌های سیستمی، مطمئن شوید وابستگی یا کاربردی برای شما ندارد.

## 4. تب Tweaks

Tweaks برای تغییر تنظیمات Windows، حذف برخی اجزای غیرضروری، تغییر سرویس‌ها، حریم خصوصی و عملکرد استفاده می‌شوند. بعضی گزینه‌ها برگشت‌پذیرند، اما برای همه تغییرات نباید روی Undo بدون Backup حساب کرد.

### Presetها

- Standard: مجموعه متعادل برای اغلب کاربران
- Minimal: حداقل تغییرات
- Advanced: تغییرات عمیق‌تر برای کاربران حرفه‌ای

## 5. تب Config

این بخش برای فعال/غیرفعال‌کردن Windows Features، اجرای Fixها، دسترسی سریع به پنل‌های قدیمی، PowerShell 7 و OpenSSH استفاده می‌شود.

## 6. تب Updates

سه حالت اصلی وجود دارد:

- Windows Default: بازگرداندن مدیریت Update به حالت عادی
- Recommended: تأخیر کنترل‌شده برای Feature/Quality Updates و جلوگیری از Restart خودکار هنگام ورود کاربر
- Disable Updates: غیرفعال‌کردن سیاست‌ها، سرویس‌ها و Taskهای Update؛ این حالت به دلیل ریسک امنیتی توصیه نمی‌شود.

## 7. Win11 Creator

ابزار Win11 Creator برای ساخت یک نصب سفارشی Windows 11 از ISO رسمی است. این فرآیند برای نصب تمیز طراحی شده، نه ارتقای In-place. ISO باید رسمی باشد و فضای موقت کافی لازم است.

## 8. روش امن پیشنهادی

برای کامپیوتر معمولی ابتدا Restore Point ایجاد کنید، سپس فقط Tweaks موردنیاز را اعمال کنید. برای شروع، Preset Minimal یا Standard از Advanced مناسب‌تر است. تغییرات مرتبط با سرویس‌ها، شبکه، Windows Update، BitLocker، Edge، OneDrive و IPv6 را آگاهانه انجام دهید.

## 9. فلسفه استفاده

WinUtil را بهتر است «جعبه‌ابزار مدیریت Windows» بدانید، نه ابزار افزایش FPS با یک کلیک. هر تغییر باید بر اساس نیاز واقعی سیستم انجام شود. اگر گزینه‌ای را نمی‌شناسید، قبل از فعال‌کردنش اثر، امکان بازگشت و وابستگی‌های آن را بررسی کنید.
