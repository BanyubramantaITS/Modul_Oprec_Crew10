# Arsitektur ROV/AUV
Bagaimana struktur urutan dari sensor ke mini pc hingga sampai ke actuator?

## Hardware
Komponen perangkat keras yang ada dalam robot bawah air.

### Mini PC

<img src="../assets/rasbpi.png" alt="Deskripsi gambar" width="640" />

Mini PC adalaha hardware pusat atau inti dari robot, dia mengerjakan semua komputasi berat seperti menjalankan ROS2, Object Detection, Pengolahan data sensor lain, dan Pengambilan keputusan behaviour Tree (Autonomous)

### Flight Controller
<img src="../assets/fc.png" alt="Deskripsi gambar" width="300" />

Flight Controller / FC adalah hardware yang berada diantara sensor/actuator dengan mini pc. Dia bertugas melakukan komputasi ringan untuk mengolah data PWM masuk dan PWM keluar antara sensor/actuator dengan mini pc.

### Sensor
<img src="../assets/sensor.jpg" alt="Deskripsi gambar" width="300" />

Komponen perangkat keras yang mendapatkan input data dari environment sekitar.

### Actuator
<img src="../assets/thruster.png" alt="Deskripsi gambar" width="300" />

Komponen perangkat keras yang mengeluarkan output.


## Diagram Utama
<img src="../assets/flowhw.png">
<img src="../assets/flowros.png">

### Jalur data naik

### Jalur data turun

### Teleop VS Otonom

## Tugas

Coba kalian buat diagram flow data ROS2 dengan tambahan pixhawk ke thruster dan menghilangkan package GUI