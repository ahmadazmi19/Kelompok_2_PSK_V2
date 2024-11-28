# Kelompok_2_PSK_V2

**A. Latar Belakang**<p>
PID Controller Motor Encoder memiliki latar belakang yang dimana dalam pengaturan rpm motor seringkali memiliki error tidak sesuai dengan rpm yang diinginkan. Dalam pembuatan PID Controller ini didasari dengan kebutuhan kontrol yang presisi dan stabilitas yang tinggi. Dengan encoder sebagai sensor feedback, PID Controller dapat menangani dinamika motor yang kompleks dan memberikan solusi fleksibel yang dapat diimplementasikan pada berbagai jenis aplikasi dan sistem. <p>

**B. Tujuan Praktikum**<p>
* Mengurangi Error
* Menyediakan Respons Cepat dan Stabil
* Menjaga Stabilitas Sistem
* Meningkatkan Efisiensi Energi
<p></p>

**C. Wiring Controller**
![Screenshot 2024-11-28 131311](https://github.com/user-attachments/assets/29cffe90-28ed-4ad3-ae96-4bf126c477d2)
<p></p>

* Hall A Phase >> D2
* Hall B Phase >> D3
* Enable A L298N >> D5
* IN1 >> D7
* IN2 >> D8
* GND Encoder >> GND
* (+)Encoder  >> 3.3V/5V
<p></p>

**D. Diagram Blok**
![Screenshot 2024-11-28 132151](https://github.com/user-attachments/assets/a0f21ab2-2d03-40ad-b9e8-f1a770eb601e)
<p></p>

1. Setpoint (Input) :nilai referensi kecepatan yang diinginkan.
2. Error (e(t)) : selisih antara setpoint dan kecepatan aktual motor.
3. Kontrol PID:
   * Kp​ menentukan seberapa besar pengaruh error pada output.
   * Ki​ menentukan seberapa cepat koreksi dilakukan.
   * Kd​ menentukan seberapa cepat sistem merespons perubahan error.
5. Keluaran PID : Ketiga komponen (P, I, D) dijumlahkan untuk menghasilkan sinyal kontrol.
6. Motor Driver : Penghubung antara sinyal Arduino dengan motor dc.
7. Motor DC : Mengubah sinyal listrik menjadi gerakan listrik dari motor driver.
8. Hall Sensor : Mengukur kecepatan aktual motor dan sebagai feedback ke kontrol PID.
   <p></p>





