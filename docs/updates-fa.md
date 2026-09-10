# Windows Update — راهنمای فارسی

## Windows Default

این حالت سیاست‌هایی را که WinUtil برای Windows Update مدیریت کرده است، به وضعیت عادی برمی‌گرداند و Startup سرویس‌ها و Scheduled Taskهای Update را اصلاح می‌کند.

**مناسب برای:** کاربری که می‌خواهد Windows Update دوباره توسط خود Windows مدیریت شود.

## Recommended

پیکربندی Recommended برای ایجاد تعادل بین دریافت به‌روزرسانی و جلوگیری از نصب/Restart ناخواسته استفاده می‌شود. طبق مستندات فعلی:

- Feature Updates تا 365 روز به تعویق می‌افتند.
- Quality Updates تا 4 روز به تعویق می‌افتند.
- Driverها از Quality Updateها مستثنا می‌شوند.
- در زمان Sign-in بودن کاربر، Scheduled Update نباید به‌صورت خودکار باعث Restart شود.
- سیاست‌های Deferred در نسخه‌های Pro، Enterprise و Education کاربرد دارند.

## Disable Updates

این حالت Policyها، Serviceها و Taskهای مرتبط با Update را غیرفعال می‌کند و فایل‌های دانلودشده Update را پاک می‌کند.

### چرا توصیه نمی‌شود؟

Windows Update علاوه بر قابلیت‌های جدید، اصلاحات امنیتی مهم دریافت می‌کند. غیرفعال‌کردن دائمی Update می‌تواند سیستم را در برابر آسیب‌پذیری‌های شناخته‌شده قرار دهد.

## پیشنهاد

اگر هدف شما جلوگیری از Restart ناگهانی یا مدیریت زمان نصب Update است، Recommended معمولاً منطقی‌تر از Disable Updates است. اگر Windows Update خراب شده، از Config > Fixes > Windows Update Reset استفاده کنید.
