# 🏭 ניהול ייצור — PWA

מערכת ניהול פקודות עבודה וייצור. עובדת מכל דפדפן, ניתנת להתקנה כאפליקציה על נייד.

---

## 🚀 העלאה ל-GitHub Pages (הכי פשוט)

### שלב 1 — צור Repository חדש
1. היכנס ל-github.com → לחץ **"New repository"**
2. שם: `pmo-production` (או כל שם שתרצה)
3. ✅ Public
4. לחץ **"Create repository"**

### שלב 2 — העלה את הקבצים
**אפשרות א׳ — דרך האתר (ללא Git):**
1. גרור את כל הקבצים לדף ה-repository
2. לחץ **"Commit changes"**

**אפשרות ב׳ — דרך Git:**
```bash
git init
git add .
git commit -m "init: pmo app"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/pmo-production.git
git push -u origin main
```

### שלב 3 — הפעל GitHub Pages
1. ב-repository לחץ **Settings** → **Pages**
2. Branch: **main** → Folder: **/ (root)**
3. לחץ **Save**
4. האפליקציה תהיה זמינה ב: `https://YOUR_USERNAME.github.io/pmo-production`

---

## 📱 התקנה כאפליקציה על נייד

### Android (Chrome)
1. פתח את הכתובת בכרום
2. תראה בנר "הוסף למסך הבית" — לחץ **הוסף**
3. האפליקציה תופיע כאייקון על המסך

### iOS (iPhone / iPad)
1. פתח בסאפארי (חובה!)
2. לחץ על כפתור **שתף** (□↑)
3. גלול מטה → **"הוסף למסך הבית"**
4. לחץ **הוסף**

---

## ☁️ חיבור Google Sheets (סנכרון בין מחשבים)

הנתונים נשמרים ב-localStorage ומסתנכרנים דרך Google Apps Script.

כדי לשנות את ה-URL, ערוך את השורה בתחילת `index.html`:
```javascript
const GS_URL="https://script.google.com/macros/s/YOUR_SCRIPT_ID/exec";
```

---

## 👤 משתמש ברירת מחדל

| שם משתמש | סיסמה    | תפקיד |
|----------|---------|--------|
| admin    | admin123 | מנהל  |

> ⚠️ שנה את הסיסמה דרך ניהול משתמשים לאחר ההתחברות הראשונה!

---

## ✨ תכונות

- 📊 דאשבורד עם KPIs, גרפים, צפי הכנסות
- 📋 ניהול פקודות עבודה מלא + פרטי אספקה
- ⚠️ מעקב חוסרים עם קבלה חלקית
- 🔧 דשבורד תקלות ייצור
- 🏗️ ניהול פרויקטים
- 📂 ייבוא / ייצוא Excel (5 גיליונות)
- 🛡️ ניהול משתמשים + הרשאות לפי פרויקט
- 📋 יומן פעילות (audit log) + undo
- ☁️ סנכרון Google Sheets
- 🌙 מצב כהה / בהיר
- 📱 PWA — ניתן להתקין על נייד
- 🔌 עובד offline (Service Worker)

---

## 📁 קבצים

| קובץ | תיאור |
|------|-------|
| `index.html` | האפליקציה המלאה |
| `manifest.json` | הגדרות PWA (שם, אייקון, צבע) |
| `sw.js` | Service Worker — תמיכה offline |
| `icon-192.png` | אייקון נייד |
| `icon-512.png` | אייקון גדול |
