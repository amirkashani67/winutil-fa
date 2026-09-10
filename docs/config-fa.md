# Config — Features و Fixes

## Windows Features

- Legacy F8 Boot Recovery: فعال/غیرفعال‌کردن رفتار قدیمی F8 برای Recovery.
- .NET Framework 2/3/4: فعال‌کردن اجزای .NET Framework موردنیاز نرم‌افزارهای قدیمی.
- Hyper-V: فعال‌کردن Hyper-V؛ ممکن است با برخی سناریوهای مجازی‌سازی دیگر تعامل داشته باشد.
- Legacy Media: فعال‌کردن اجزای قدیمی مانند Windows Media Player/DirectPlay در سیستم‌های سازگار.
- NFS: فعال‌کردن قابلیت NFS.
- Registry Backup: تنظیم پشتیبان‌گیری زمان‌بندی‌شده Registry؛ زمان پیش‌فرض مستندشده 12:30 شب است.
- Windows Sandbox: فعال‌کردن Sandbox در نسخه‌های پشتیبانی‌شده.
- WSL: فعال‌کردن Windows Subsystem for Linux.

## Fixes

- AutoLogon: تنظیمات AutoLogon را مدیریت می‌کند؛ برای سیستم‌های حساس با احتیاط.
- System Corruption Scan: اجرای بررسی و ترمیم خرابی فایل‌های سیستم.
- Network Reset: بازنشانی اجزای شبکه؛ ممکن است تنظیمات شبکه سفارشی را از بین ببرد.
- NTP Server Enable: فعال‌سازی نقش/تنظیمات مرتبط با NTP Server.
- Windows Update Reset: بازنشانی مؤلفه‌های Windows Update.
- WinGet Reinstall: تلاش برای نصب مجدد WinGet در صورت خرابی.

## Legacy Panels

WinUtil میانبرهایی برای پنل‌های قدیمی Windows فراهم می‌کند، از جمله:

Computer Management، Control Panel، Defender Firewall، Mouse Properties، Network Connections، Power Panel، Printer Panel، Programs and Features، Region، Windows Restore، Security and Maintenance، Sound Settings، System Properties، Time and Date و User Accounts.

## PowerShell 7

امکان نصب/حذف پروفایل PowerShell 7 در WinUtil وجود دارد. برای رفع برخی مشکلات DISM، نسخه Microsoft Store به‌صورت MSIX ممکن است مشکل «Class not registered» ایجاد کند؛ در چنین شرایطی نسخه WinGet/MSI انتخاب مناسب‌تری است.

## OpenSSH

گزینه OpenSSH Server Enable برای فعال‌کردن OpenSSH Server در Windows استفاده می‌شود. پس از فعال‌سازی، تنظیم Firewall و احراز هویت را نیز بررسی کنید.

## نکته عیب‌یابی

Fixها را به‌عنوان آخرین راه‌حل کور اجرا نکنید. ابتدا مشخص کنید مشکل مربوط به Windows Update، شبکه، فایل‌های سیستمی یا WinGet است؛ سپس Fix متناسب را اجرا کنید.
