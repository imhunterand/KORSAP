# KORSAP
**KORSAP** adalah alat yang kuat dan berguna yang dapat digunakan untuk menemukan kamera pengintai keamanan IP dengan port terbuka di seluruh dunia. Untuk menemukan kamera IP, alat ini menggunakan API mesin pencari Shodan. Dan menggunakan Shodan Premium, hanya menargetkan kamera pengintai video berdasarkan merek tertentu. Setelah kamera IP ditemukan, script akan mencoba mengeksploitasi koneksi ke perangkat menggunakan kredensial default rekanan. 
Private Camera Exploitation (KoruptorSadap) 🎥

![hayongapain](https://user-images.githubusercontent.com/109766416/184430571-61240e51-37bb-4f8e-b3a0-562279793175.gif)


Saat ini hanya 3 jenis merek kamera pengintai keamanan IP yang didukung, Sony, Canon dan Panasonic. Tapi saya mungkin berencana untuk menambahkan merek berikut dalam waktu dekat: Alphafinity, INSTAR, Milesight, Vacron dan VideoIQ.

Ada juga fungsi ekspor yang memberikan kemungkinan untuk menyimpan hasil penelitian dalam format `.csv` atau `.txt` setelah selesai.

# Konsep Installation:


**Requirement**
 * Python 3 (Tested with Python 3.8.5)
 * Shodan Account (Premium API key)

**Installation**
Clone this repository and run:
```
pip install -r requirements.txt
```
Usage
```
python3 korsap.py
```

[![ALT](https://youtube-md.vercel.app/0gXyyBiX8Ak)](https://www.youtube.com/watch?v=0gXyyBiX8Ak)

# List of Dorks
Banyak dari dorks dapat dimodifikasi untuk membuat pencarian lebih spesifik atau generik.

Brand          | Dork                                     | Default Credentials      | Description
-------------|-----------------------------------|--------------------------|------------------------------------------------
Panasonic |title:"network camera" | admin/12345 | Ex: WV-SW316, BB-ST165, BL-VP101...
Canon     |title:"network camera vb-" | root/camera | Ex: VB-H761LVE, VB-R13, VB-H651V...
Sony      |title:"Sony Network Camera" | admin/admin | Ex: SNC-EM602R, SNC-CX600W, SNC-EB642R...
INSTAR |title:"INSTAR Full-HD IP-Camera" | admin/instar | INSTAR?
VideoIQ |title:"VideoIQ Camera Login"  | admin/admin | VideoIQ?
Milesight |title:"Milesight Network Camera" | admin/ms1234 | Milesight?
Vacron |title:"Milesight Network Camera" | admin/admin | Vacron?
Alphafinity |title:"Alphafinity Network Camera" | admin/admin | Alphafinity?
