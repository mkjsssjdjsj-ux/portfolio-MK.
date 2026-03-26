# نسخة جاهزة للنشر

أنا جهزت لك المشروع في صورة Vite + React + Firebase.

## المطلوب منك فقط

1. افتح Firebase واعمل مشروع جديد.
2. فعّل:
   - Firestore Database
   - Authentication > Anonymous
   - Hosting
3. انسخ ملف `.env.example` وسمّه `.env`.
4. حط بيانات Firebase الحقيقية داخل `.env`.
5. افتح التيرمنال داخل المجلد وشغّل:

```bash
npm install
npm run build
npm install -g firebase-tools
firebase login
firebase use --add
firebase deploy
```

## ملاحظات مهمة

- الموقع جاهز للنشر، لكن لا يمكنني أنا أسجل دخول بحساب Firebase الخاص بك أو أنشر بدلًا منك بدون وصول لحسابك.
- كلمة سر الأدمن الموجودة داخل الكود ليست آمنة للإنتاج، لكنها ستعمل مؤقتًا كما هي.
- الرسائل تتخزن في Firestore، وليست إرسالًا مباشرًا للإيميل.

## ملف البيئة

أنشئ ملف `.env` بجوار `package.json` مثل هذا:

```env
VITE_FIREBASE_API_KEY=your_api_key
VITE_FIREBASE_AUTH_DOMAIN=your-project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your-project-id
VITE_FIREBASE_STORAGE_BUCKET=your-project.firebasestorage.app
VITE_FIREBASE_MESSAGING_SENDER_ID=123456789
VITE_FIREBASE_APP_ID=1:123456789:web:abcdef123456
VITE_PORTFOLIO_APP_ID=mohamed-khaled-portfolio
```
