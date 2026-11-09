چادرها — نسخه Web App کیهانی

اجرا:
1) فایل ZIP را استخراج کنید.
2) پوشه chadorha-webapp را روی یک هاست استاتیک با HTTPS منتشر کنید (مثلاً Netlify، Vercel یا GitHub Pages).
3) آدرس سایت را در مرورگر موبایل باز کنید.
4) از دکمه «نصب وب‌اپ» یا گزینه Install app / Add to Home Screen مرورگر استفاده کنید.

برای تست محلی با پایتون:
  cd chadorha-webapp
  python -m http.server 8080
سپس در مرورگر باز کنید:
  http://localhost:8080

نکته:
- برای نصب PWA، فایل‌ها باید از HTTPS یا localhost سرو شوند؛ باز کردن مستقیم index.html به‌صورت file:// امکان نصب کامل و Service Worker را نمی‌دهد.
- بازی بدون اینترنت هم پس از اولین بارگذاری موفق، با Service Worker در دسترس می‌ماند.
- پیشرفت بازی در localStorage همان مرورگر/دستگاه ذخیره می‌شود و هنوز همگام‌سازی ابری یا حساب کاربری ندارد.
