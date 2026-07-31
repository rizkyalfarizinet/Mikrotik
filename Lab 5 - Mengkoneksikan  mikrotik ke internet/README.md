  <h2>LAB 5</h2>
  <h3>Mengkoneksikan  mikrotik ke internet</h3>

Bismillahirohmaanirrohiim, Assalamu’alaikum Warrohmatullohi Wabarokatuh
  <img width="550" height="350" alt="topologi basic" src="https://github.com/user-attachments/assets/b0999885-6bbe-4ba9-aaac-6ab9e03ecf74" />
  
Perintah konfigurasi  mikrotik ke internet  dengan IP dynamic
  - Pasangkan pengkabelan LAN sesuai dengan topologi di atas
  - Setting nama interface Routerboard Mikrotik:
     ether1-WAN (untuk koneksi ke Internet), dan 
     ether2-LAN (untuk koneksi ke PC Klien)
    <img width="673" height="175" alt="Cuplikan layar 2026-07-31 150554" src="https://github.com/user-attachments/assets/b4e2b190-5676-4274-a022-9de53bb93592" />

  - Konfigurasi DHCP Client ether1-WAN agar dapat IP dari dari Router Telkom/ISP/Internet
    IP > DHCP Client
    + Interface= ether1-WAN
    Apply
    OK
    <img width="706" height="242" alt="Cuplikan layar 2026-07-31 151220" src="https://github.com/user-attachments/assets/f79061b6-a0b2-4ef8-80ad-4872b17ebf97" />


