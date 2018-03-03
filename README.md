# exemplo-android

## Configuração da licenca no ANDROID_HOME do linux

<pre>
./tools/bin/sdkmanager "platform-tools" "platforms;android-26"
</pre>

## Gerar certificado
<pre>
keytool -genkey -v -keystore franciscocalaca.keystore -alias app1 -keyalg RSA -keysize 2048 -validity 10000
</pre>

## Assinar um APK

<pre>
/home/aluno/android/build-tools/26.0.2/apksigner sign --ks-pass pass:123456 --ks /home/aluno/android/franciscocalaca.keystore --out my-app-release.apk app/build/outputs/apk/release/app-release-unsigned.apk
</pre>
