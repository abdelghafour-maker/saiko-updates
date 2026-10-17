# Saiko no Sushi — Update Feed / خادم التحديثات

هذا المستودع **ليس شيفرة المصدر** — إنه فقط مساحة عامة لتحديثات تطبيق
**Saiko no Sushi Desktop** التلقائية.

This repository is **not the source code** — it only hosts the automatic
update feed (installers + metadata) for the Saiko no Sushi Desktop app.

## مصدر التحديث / Update feed

```
https://github.com/abdelghafour-maker/saiko-updates/releases/latest/download/
```

The app checks this URL on startup and every 30 minutes, then downloads and
installs the newer version automatically.

## الملفات في كل إصدار / Assets per release

| الملف | الوصف |
|---|---|
| `latest.yml` | بيانات الإصدار (version + sha512 + size) |
| `saikonosushi Desktop Setup X.Y.Z.exe` | ملف التثبيت (NSIS) |
| `...exe.blockmap` | خريطة الكتل (للتحميل التفاضلي) |

## تنبيه / Warning

لا تحذف الإصدارات (releases) ولا تعدّل أسماء الملفات — التطبيق يعتمد عليها
حرفيًا. النشر يتم آليًا عبر السكربت:

```
D:\siteweb\studio-feed\publish-online.ps1
```