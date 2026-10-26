# فلوسي - مشروع الـ APK

التطبيق (index.html) جوّا الـ APK نفسه، فبيشتغل من غير إنترنت وبياناتك بتتحفظ على التليفون.

## الطريقة 1: من غير Android Studio (GitHub)
1. اعمل حساب على github.com وأنشئ Repository جديد.
2. ارفع كل ملفات المشروع (Add file > Upload files).
3. لو فولدر .github اتخطّى، اعمل ملف جديد (Add file > Create new file) باسم
   .github/workflows/build.yml وألزق جواه محتوى الملف الموجود في المشروع.
4. من تبويب Actions شغّل Build APK (Run workflow)، واستنى كام دقيقة.
5. افتح التشغيلة الناجحة ونزّل RiderMoney-apk (جواها app-debug.apk) وثبّته على الموبايل.
   (لازم تسمح بتثبيت التطبيقات من مصدر غير معروف.)

## الطريقة 2: Android Studio
1. افتح المجلد في Android Studio وانتظر Gradle Sync.
2. Build > Build APK(s)، والملف بيظهر في app/build/outputs/apk/debug/app-debug.apk

## تحديث التطبيق
عدّل app/src/main/assets/index.html (الصق النسخة الجديدة) وابنِ الـ APK من جديد.
بياناتك بتفضل لو ثبّتت النسخة الجديدة فوق القديمة (من غير ما تمسح التطبيق الأول).

## ملاحظة
زرار "اقرأ الأرقام من صورة" مش هيظهر جوّا الـ APK، لأنه بيحتاج Claude. باقي المميزات شغالة.
