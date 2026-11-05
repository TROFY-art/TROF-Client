TROF Client - Zalith rebrand patch (ضعه فوق مستودع Zalith بعد عمل Fork)
- ZalithLauncher/gradle.properties : الاسم TROF Client
- .github/workflows/android.yml    : بناء APK تلقائي على حسابك (arm64 debug)
- res/mipmap-*/ic_launcher*.png    : أيقونة التطبيق (شعار TF)
- res/drawable/ic_launcher_background.xml
- res/drawable/app_name_title.png  : شعار صفحة "حول"
Termux:
  git clone https://github.com/USERNAME/ZalithLauncher && cd ZalithLauncher
  unzip -o /sdcard/Download/trof_zalith_patch.zip -d /tmp/p
  cp -r /tmp/p/trof_zalith_patch/. .
  git add -A && git commit -m "TROF rebrand" && git push
ثم GitHub > Actions > Build TROF Client > Run workflow > Artifacts
