### Aktifkan trackpad di hackintosh Menggunakan Appleps2smarttouchpad.kext

> ⚠️ Kext ini mengemulasi beberapa gerakan dengan mengirimkan sistem dengan pintasan keyboard yang sesuai. Misalnya, setelah kext mendeteksi gesekan tiga jari ke kiri, ia akan memasukkan kontrol + kiri untuk beralih ruang kerja. Ini berfungsi dengan baik tetapi sedikit kikuk (Anda tidak dapat memindahkan ruang kerja setengah jalan untuk melihat apa yang ada di yang lain misalnya)

> ⚠️ ***Repo ini hanya membantu menyalakan gerakan beberapa gesture saja***. Bagian terbaiknya, **KEMUNGKINAN** setiap gerakan bekerja seperti yang dijelaskan

### Fitur yang Didukung
- Mode mouse dengan Tombol Virtual Kiri, Kanan dan Tengah
- Mengetuk -  Hingga 5 jari
- Mengklik - Hingga 5 jari
- Menyeret: Ketuk untuk melepaskan dan Angkat Jari 
- Ketuk Sudut
- Menggulir - Tepi satu jari dan gesek Dua Jari
- Efek gulir terus menerus, Linear, Sling dan Inersia
- Finger Press - Hingga 5 jari
- Menggesek - Ujung, Tiga dan Empat Jari
- Zoom - Zoom cubit dengan dua jari, Zoom OSX dengan Keyboard
- 4 (Elan, Focaltech) & 5 jari Gerakan mencubit
- Rotasi - Rotasi Busur dan Gesek
- Input/Telapak Tangan yang Tidak Disengaja saat mengetik

<details>
  <summary>Preview :</summary>
<p align="center">
  <kbd>
  <img src="https://github.com/JaemanPratama/Appleps2smarttouchpad-gesture-settings/blob/main/IMG/anim1.gif" alt="animated" />
    </kbd>
</p>
</details>


```
Source :
Elan & Smart Touchpad Ps2 https://osxlatitude.com/forums/topic/1948-elan-focaltech-and-synaptics-smart-touchpad-driver-mac-os-x/
VoodooPS2 by Acidanthera https://github.com/acidanthera/VoodooPS2/releases
```

```
Di laptop saya, saya melihat kontrol trackpad tetapi hanya menggesek ke atas dan ke bawah dengan gerakan dua jari yang berfungsi. Gerakan lain ditampilkan di pengaturan Trackpad tetapi tidak berfungsi sama sekali. Jika demikian halnya dengan Anda, ikuti panduan ini dan ini pasti akan memperbaiki masalah.
```

#### 🧭 Langkah-langkahnya sederhana. Yang harus Anda lakukan adalah mengunduh paket [ApplePS2SmartTouchPad.kext.zip](https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/releases) . Setelah mengunduh paket, ikuti langkah-langkah ini:

1. Hapus  kext "ApplePS2Controller, VoodooPS2Controller, AppleACPIPS2Nub, ApplePS2Keyboard, dan Elan Touchpad lama"  yang ada jika Anda telah menginstal dari HDD  `/System/Library/Extensions` ,   `/Extra/Extensions`
2. Gunakan mounter EFI atau aplikasi konfigurator OC untuk memasang partisi EFI
3. Ekstrak paket ApplePS2SmartTouchPad. Folder yang diekstrak berisi 1 file kext
4. Sekarang tergantung pada jenis trackpad Anda yaitu mencari tahu dari Windows Device Manager
5. salin ApplePS2SmartTouchPad.kext folder `EFI > OC > Kexts` dan reboot sistem.

#### 🔍 Konfigurasi Prefensi System :

1. Prefensi System -> Aksebilitas -> Kontrol Petunjuk -> Pilihan Trackpad Dan Centang Aktifkan penyeretan :

`Prefensi System`|`Aksebilitas`|`Kontrol Petunjuk`|`Pilihan Trackpad`|`Aktifkan penyeretan`
---|---|---|---|---
<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/ICON%201.png"/>|<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/IMG%201.png"/>|<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/IMG%202.png"/>|<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/IMG%203.png"/>|<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/IMG%204.png"/>

2. Prefensi System -> Trackpad -> Centang ketuk Untuk Mengeklik :

`Prefensi System`|`Trackpad`|`Centang ketuk Untuk Mengeklik`|`Extra`
---|---|---|---|
<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/ICON%201.png"/>|<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/IMG%205.png"/>|<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/IMG%206.png"/>|<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/IMG%207.png"/> ***Bagi mereka yang ingin Scroll Touchpad Terbalik (Seperti Windows) Hapus Centang Arah Gulir Alami***


3. Prefensi System -> Papan Ketik -> Edit Sesuai Dengan Tombol Shorchut dibawah Ini :

`Prefensi System`|`Papan Ketik`|`Launchpad`|`Mission Control`
---|---|---|---|
<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/ICON%201.png"/>|<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/IMG%208.png"/>|<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/IMG%209.png"/>|<img src ="https://github.com/JaemanPratama/Kext-Elan-ETD0108-PS-2-Interface-Trackpad/blob/main/IMG/IMG%2010.png"/>|


### Berikut Ini adalah fitur yang Bisa Anda Dapatkan Setelah Mengedit di Bagian Prefensi System :



Gesture             |  Deskripsi
:-------------------------:|:-------------------------:
![](https://help.apple.com/assets/61B3707D08121F6CC14EE202/61B3708108121F6CC14EE219/en_US/e4ec3f469848fb67d38456b3e8102841.png)  |  Klik. Tekan dengan satu jari sampai Anda merasakan bunyi klik
![](https://help.apple.com/assets/61B3707D08121F6CC14EE202/61B3708108121F6CC14EE219/en_US/56ec4624f733aee607452836e1297620.png) | Klik dan tahan. Tekan dan tahan dengan satu jari
![](https://help.apple.com/assets/61B3707D08121F6CC14EE202/61B3708108121F6CC14EE219/en_US/43a977c6ccd44e79d4f23d2afce87ea2.png) | Drag and Drop. Klik dan tahan item, lalu geser jari Anda melintasi trackpad untuk memindahkannya
![](https://help.apple.com/assets/61B3707D08121F6CC14EE202/61B3708108121F6CC14EE219/en_US/f2228a48e840ef8dd679a2e8d3d3cb8c.png) | Gulir ke atas atau ke bawah. Geser dua jari ke atas atau ke bawah
![](https://help.apple.com/assets/61B3707D08121F6CC14EE202/61B3708108121F6CC14EE219/en_US/b83e057e5c55307d64bd75f18e62d954.png) | Gulir ke kiri atau kanan. Geser dua jari ke kiri atau kanan
![](https://help.apple.com/assets/61B3707D08121F6CC14EE202/61B3708108121F6CC14EE219/en_US/72c3dd13054b11eb8793d12de4738d03.png) | Perbesar. Letakkan dua jari di dekat satu sama lain. Cubit terbuka untuk memperbesar, atau cubit tertutup untuk memperkecil (**Rusak**)
![](https://help.apple.com/assets/61B3707D08121F6CC14EE202/61B3708108121F6CC14EE219/en_US/2b85d08fbce2e3021bb86ebc9b52c751.png) | Membuka Mission Control. Geser ke atas dengan tiga jari
![](https://help.apple.com/assets/60956BCCB4EAF4452A503181/60956BCDB4EAF4452A50318F/en_US/080f756e0c8b56c2e7a2c925b1a01a96.png) | Membuka APP EXPOSE. Geser ke bawah dengan tiga jari 
![](https://help.apple.com/assets/61B3707D08121F6CC14EE202/61B3708108121F6CC14EE219/en_US/32be9f6360ff6ae5bddd592b4f398358.png) | Beralih di antara aplikasi yang terbuka. Geser ke kiri atau kanan dengan tiga jari untuk berpindah antara desktop dan aplikasi layar penuh
![](https://help.apple.com/assets/61B3707D08121F6CC14EE202/61B3708108121F6CC14EE219/en_US/f3f6cfb1e34037ce6afdb601497123e8.png) | klik kanan.  Klik atau ketuk dengan dua jari 
![](https://support.apple.com/library/content/dam/edam/applecare/images/en_US/keyboards/trackpad2-open-notification-center.png) | Buka Pusat Pemberitahuan. Gesek ke kiri dari tepi kanan dengan dua jari untuk menampilkan Pusat Pemberitahuan
![](https://support.apple.com/library/content/dam/edam/applecare/images/en_US/keyboards/trackpad2-smart-zoom.png) | ~~Zoom cerdas. Ketuk dua kali dengan dua jari untuk memperbesar dan memperkecil halaman web atau PDF~~
![](https://user-images.githubusercontent.com/89202419/160249799-bb17e9d2-3031-41b3-a38c-f5eff9c69eaa.png) | Menampilkan Desktop. Klik 5 jari untuk menampilkan Desktop
![](https://support.apple.com/library/content/dam/edam/applecare/images/en_US/keyboards/trackpad2-launchpad.png) | Membuka Launchpad. Jepit 5 jari untuk Menampilkan Launchpad
![](https://user-images.githubusercontent.com/89202419/161056439-231fdc0c-1984-449f-bee6-00d10e1c6ee2.jpg)| Ketukan Sudut. Mengetuk di area sudut touchpad
![](https://user-images.githubusercontent.com/89202419/161057779-12b20f1a-6a6b-401d-8265-d0677a448832.png) |  Rotasi. letakkan jari pertama di touchpad selama 1-2 detik sebelum memutar dengan jari lain
![](https://user-images.githubusercontent.com/89202419/161063663-8925e6cd-1907-4ffc-99d3-d5ea65468867.png) | Klik Tengah. Emulasi Klik Tengah Seperti Pada Mouse
