  <h2>LAB 5</h2>
  <h3>Mengkoneksikan  mikrotik ke internet</h3>

Bismillahirohmaanirrohiim, Assalamu’alaikum Warrohmatullohi Wabarokatuh<br>
  <img width="550" height="350" alt="topologi basic" src="https://github.com/user-attachments/assets/b0999885-6bbe-4ba9-aaac-6ab9e03ecf74" />
  
Perintah konfigurasi  mikrotik ke internet  dengan IP dynamic
  - Pasangkan pengkabelan LAN sesuai dengan topologi di atas
  - Setting nama interface Routerboard Mikrotik:
     ether1-WAN (untuk koneksi ke Internet), dan 
     ether2-LAN (untuk koneksi ke PC Klien)
    <img width="673" height="175" alt="Cuplikan layar 2026-07-31 150554" src="https://github.com/user-attachments/assets/b4e2b190-5676-4274-a022-9de53bb93592" />

  - Konfigurasi DHCP Client ether1-WAN agar dapat IP dari dari Router Telkom/ISP/Internet
    IP > DHCP Client
    + Interface= ether1-WAN<br>
    Apply<br>
    OK<br>
  
    <img width="706" height="242" alt="Cuplikan layar 2026-07-31 151220" src="https://github.com/user-attachments/assets/f79061b6-a0b2-4ef8-80ad-4872b17ebf97" />

    Cek pada tab status, lihat IP yang didapatkan oleh ether1-WAN
    <img width="707" height="243" alt="Cuplikan layar 2026-07-31 151324" src="https://github.com/user-attachments/assets/1f223a64-4e06-4adb-8fed-e7b704c8c40b" />

 - pengecekan koneksi dari Mikrotik ke Internet
   Terminal: 
   <img width="468" height="299" alt="Cuplikan layar 2026-07-31 151955" src="https://github.com/user-attachments/assets/c46320fa-2fe7-4cc4-8c59-ad953cf19b20" />

    Alhamdulillaah, Mikrotik sudah terkoneksi ke Internet

 - Lakukan seting IP pada interface ether2-LAN
   IP > Address<br>
   + Address= 192.168.10.1/24<br>
   Interface=  ether2-LAN<br>
   Apply<br>
   OK<br>
   <img width="497" height="117" alt="Cuplikan layar 2026-07-31 152505" src="https://github.com/user-attachments/assets/a87cb8f2-0ad3-4e72-92cf-78e1541b0f3d" />


 - Lakukan konfigurasi NAT, agar PC Klien dapat terkoneksi Internet melewati Mikrotik:
    IP > Firewall > 
    <img width="506" height="115" alt="Cuplikan layar 2026-07-31 152838" src="https://github.com/user-attachments/assets/42f36f93-eba6-4be7-a4da-66fb936039e5" />
<br>
<br>
<br>
 - Kesimpulan

 Berdasarkan praktikum yang telah dilakukan, konfigurasi DHCP Client pada interface ether1 berhasil memperoleh alamat IP secara otomatis dari DHCP Server. Selanjutnya dilakukan pengujian koneksi menggunakan perintah ping google.com melalui Terminal MikroTik, dan hasilnya berhasil (reply), sehingga menunjukkan koneksi internet telah aktif.

 Selain itu, telah dilakukan konfigurasi IP Address beserta Subnet Mask pada interface jaringan lokal serta penambahan aturan Firewall (NAT Masquerade) agar jaringan lokal dapat mengakses internet. Dengan demikian, seluruh konfigurasi berjalan dengan baik dan MikroTik berhasil menghubungkan jaringan lokal ke internet menggunakan IP Dynamic (DHCP Client).


