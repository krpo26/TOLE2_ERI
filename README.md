# TOLE2_ERI
App offline de anatomía ósea (Capacitor + HTML). Admin: contraseña en www/index.html (const PW).

## 1. GitHub
git init && git add . && git commit -m "TOLE2_ERI"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/TOLE2_ERI.git
git push -u origin main

## 2. Codemagic (APK)
codemagic.io → Add application → GitHub → TOLE2_ERI → Android/codemagic.yaml → Start build.
El APK aparece en Artifacts y llega por correo.
Para publicar en Play Store hay que añadir firma (keystore) en Codemagic → Code signing.

## 3. Firebase (opcional)
npm i -g firebase-tools && firebase login && firebase init hosting (carpeta www)
firebase deploy   # versión web
APK: Firebase Console → App Distribution para repartir el APK a testers.
