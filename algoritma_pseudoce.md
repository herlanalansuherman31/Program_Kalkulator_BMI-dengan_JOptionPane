# Pseudocode Program Kalkulator BMI 
## judul:
algoritma kalkulator bmi
## deklarasi
**var** bb ,tb ,konversi ,bmi = double
**var** inputBB, inputTB, kategori, hasil = string
## algoritma:
BEGIN

    TAMPILKAN_PROMPT("Masukkan berat badan (kg):")
    READ (inputBB)
    
    TAMPILKAN_PROMPT("Masukkan tinggi badan (cm):")
    READ (inputTB)
    bb = konversudouble(inputBB)
    TB = konvesrsidouble(inputTB)
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
        kategori = "Tidak Normal"
        
    hasil = "Berat Badan: " + bb + "kg" + "Tinggi Badan: " + TB + "cm" + "Nilai BMI: " + BMI + "Kategori: " + kategori
            
    WRITE("Hasil Perhitungan BMI Anda:", hasil)

END
