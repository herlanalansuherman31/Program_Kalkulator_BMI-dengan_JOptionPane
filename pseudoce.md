# Pseudocode Program Kalkulator BMI 
## judul:
algoritma kalkulator bmi
## deklarasi
**var** bb ,tb ,konversi ,bmi = double
**var** inputBB, inputTB, kategori, hasil = string
## algoritma:
BEGIN
    TAMPILKAN_PROMPT("Masukkan berat badan (kg):")
    READ inputBB 
    TAMPILKAN_PROMPT("Masukkan tinggi badan (cm):")
    READ inputTB 
    konversi = TB / 100 // konversi dari cm ke meter
    BMI = bb / (konversi * konversi)
    JIKA (BMI < 18.5) MAKA
        kategori = "kurus"
    SEBALIKNYA JIKA (BMI < 24.9) MAKA
        kategori = "normal"
    SEBALIKNYA JIKA (BMI < 29.9) MAKA
        kategori = "gemuk"
    SEBALIKNYA JIKA (BMI > 30.0) 
        kategori = "obesitas"
    SELAIN ITU
        kategori = "Tidak Diketahui/Tidak Normal
    hasil = "Berat Badan: " + bb + "kg" + BARIS_BARU + 
            "Tinggi Badan: " + TB + "cm" + BARIS_BARU + 
            "Nilai BMI: " + BMI + BARIS_BARU + 
            "Kategori: " + kategori
    WRITE("Hasil Perhitungan BMI Anda:", hasil)

END
