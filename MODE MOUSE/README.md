### MOUSE MODE

Pada Dasarnya kext ini hanya mengemulasi kan untuk bertindak seperti mouse dengan tiga tombol kiri, kanan dan tengah dan mengarahkan kursor. 

```
TOMBOL: 
Tombol kiri :    Melakukan klik kiri
Tombol kanan :    Melakukan klik kanan
Tombol tengah :    Melakukan klik tengah
```

```
Untuk klik Tengah: 
Click-pad : Tekan dan klik di tengah area tombol touchpad
Touchpad dengan tombol fisik kiri dan kanan : Klik tombol kiri dan kanan secara bersamaan
```

Kustomisasi:

Anda dapat mengontrol tombol dengan opsi daftar berikut. Terletak di  `IOKitPersonalities -> Smart-Pad -> Preferences -> Buttons`  di plist :

 `ClickpadVirtualButtons` (Yes / No) : Mengaktifkan tombol virtual untuk click-pads dengan membagi area bawah menjadi tiga bagian, jika tidak, hanya satu tombol "Kiri" yang akan berfungsi secara default.

`ClickpadVirtualButtonsArea` (Nilai 0 -100) : Menyetel % area touchpad (bawah) yang digunakan oleh tombol virtual. 
<details>
<summary></summary>
<img src="https://github.com/JaemanPratama/Appleps2smarttouchpad-gesture-settings/blob/main/IMG/m1.png" width="50%" height="50%">
</details>

`DisablePhysicalClicks` (Yes / No): Mengaktifkan/Menonaktifkan tombol fisik.

`VirtualMiddleButton` (Yes / No): Mengaktifkan/Menonaktifkan tombol tengah virtual untuk click-pad.

