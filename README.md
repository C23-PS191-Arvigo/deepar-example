## Install library Deepar ke project

1. Membuat folder `deepar` untuk `deepar.aar` di root direktori
2. Masukan implementation library Deepar ke `build.gradle`
   - implementation files("../deepar/deepar.aar")
3. Sinkron ulang `gradle`
4. Memastikan library berhasil di tambahkan ke project
   - File -> Project Structure... -> app -> `../deepar/deepar.aar`

## Import dari library DeepAR yang akan digunakan

1. import ai.deepar.ar.ARErrorType; 
2. import ai.deepar.ar.AREventListener;
3. import ai.deepar.ar.CameraResolutionPreset;
4. import ai.deepar.ar.DeepAR;
5. import ai.deepar.ar.DeepARImageFormat;

## Function initialize yang digunakan di MainActivity

1. initializeDeepAR(); // Untuk inisialisasi license key dari DeepAR
2. initializeFilters(); // Untuk inisialisasi filter dari DeepAR yang akan digunakan
3. initalizeViews(); // Untuk inisialisasikan DeepAR agar dapat ditampilkan ke kamera

## API dari library DeepAR yang akan digunakan

1. deepAR.getExternalGlTexture()
2. deepAR.receiveFrameExternalTexture()
3. deepAR.takeScreenshot()
4. deepAR.setLicenseKey()
5. deepAR.initialize()
6. deepAR.receiveFrame()
7. deepAR.switchEffect()
8. deepAR.release()
9. deepAR.setAREventListener()
10. deepAR.setRenderSurface()

## [Referensi/Penjelasan API dari DeepAR](https://s3.eu-west-1.amazonaws.com/sdk.developer.deepar.ai/doc/android/index.html)

## Permission yang digunakan

1. Camera - `android.permission.CAMERA`
2. External file storage - `android.permission.WRITE_EXTERNAL_STORAGE`
3. Record audio - `android.permission.RECORD_AUDIO`

## ProGuard untuk DeepAR

`-keepclassmembers class ai.deepar.ar.DeepAR { *; }`

## [Dokumentasi DeepAR](https://docs.deepar.ai/deepar-sdk/deep-ar-sdk-for-android/getting-started/)


