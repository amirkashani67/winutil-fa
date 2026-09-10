# راهنمای فارسی WinUtil

> مستندات و آموزش فارسی **Chris Titus Tech's Windows Utility (WinUtil)**

این مخزن برای ارائه یک راهنمای فارسی، دقیق و آموزشی برای WinUtil ایجاد شده است. کد اصلی WinUtil در این مخزن کپی یا دستکاری نمی‌شود.

## WinUtil چیست؟

WinUtil مجموعه‌ای از ابزارهای مدیریتی Windows برای نصب و مدیریت برنامه‌ها، اعمال Tweaks، عیب‌یابی، تنظیم قابلیت‌های Windows و مدیریت Windows Update است.

## شروع سریع

WinUtil را با **PowerShell یا Windows Terminal با دسترسی Administrator** اجرا کنید.

### نسخه پایدار — پیشنهادشده

```powershell
irm https://christitus.com/win | iex
```

### نسخه توسعه

```powershell
irm https://christitus.com/windev | iex
```

### اجرای خودکار Preset

```powershell
& ([ScriptBlock]::Create((irm https://christitus.com/win))) -Preset Standard
```

Presetهای اصلی شامل `Standard`، `Minimal` و `Advanced` هستند.

## فهرست راهنما

### آموزش و استفاده

- [راهنمای جامع](docs/guide-fa.md)
- [Applications — مدیریت برنامه‌ها](docs/applications-fa.md)
- [Tweaks و توضیح گزینه‌ها](docs/tweaks-fa.md)
- [Config، Features و Fixes](docs/config-fa.md)
- [Windows Update](docs/updates-fa.md)
- [Win11 Creator](docs/win11-creator-fa.md)
- [Automation و Presetها](docs/automation-fa.md)
- [FAQ، خطاهای متداول و نکات ایمنی](docs/faq-fa.md)

### برای توسعه‌دهندگان

- [ساختار فنی پروژه](docs/architecture-fa.md)

## هشدار مهم

WinUtil می‌تواند تنظیمات سطح سیستم را تغییر دهد. قبل از اعمال Tweaks مهم، Restore Point یا Backup مناسب داشته باشید. گزینه‌هایی مانند حذف OneDrive، حذف Edge، تغییر IPv6، غیرفعال‌کردن Windows Update یا تغییر سرویس‌ها را فقط با شناخت اثرات آن‌ها اجرا کنید.

## پشتیبانی Windows

طبق مستندات فعلی پروژه اصلی، WinUtil برای **Windows 11** پشتیبانی می‌شود. Windows 10 به‌دلیل پایان پشتیبانی رسمی مایکروسافت در 14 اکتبر 2025 دیگر هدف پشتیبانی پروژه نیست.

## منابع رسمی

- پروژه اصلی: https://github.com/ChrisTitusTech/winutil
- مستندات رسمی: https://winutil.christitus.com/
- Known Issues: https://winutil.christitus.com/knownissues/

## انتساب

WinUtil یک پروژه متعلق به Chris Titus Tech است. این مخزن با هدف تهیه مستندات فارسی و آموزشی ایجاد شده است. برای کد، مجوز و شرایط استفاده از پروژه اصلی، به مخزن رسمی مراجعه کنید.
