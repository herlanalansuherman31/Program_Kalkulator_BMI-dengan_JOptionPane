#  🧮Program Kalkulator BMI dengan JOptionPane

## 👤 Identitas
- **Nama:** HERLAN ALAN SUHERMAN
- **NIM:** I.2510319
- **Mata Kuliah:** Algoritma dan Pemrograman  

---

## 🧠 Deskripsi
Program ini menghitung **Indeks Massa Tubuh (BMI)** berdasarkan **berat badan (kg)** dan **tinggi badan (cm)** menggunakan **JOptionPane** untuk input dan output.  
Langkah program:
1. Pengguna memasukan berat badan dan tinggi badan
2. Program akan mengkonversi terlebih dahulu tinggi badan dari cm ke m
3. program menghitung hasil bmi 
4. Hasil ditampilkan dalam kotak dialog  

---

## 💻 Cuplikan Kode
```java
package com.example;

import javax.swing.JOptionPane;
//contoh dasar kalkulator bmi
public class KalkulatorBMI {

	public static void main(String[] args) {
		String inputBB = JOptionPane.showInputDialog("masukan berat badan(kg):");
		String inputTB = JOptionPane.showInputDialog("masukan tinggi badan(cm):");
		double bb = Double.parseDouble(inputBB); //mengkonversi string ke double
		double TB = Double.parseDouble(inputTB); //mengkonversi string ke double
		double konversi = TB / 100; //mengkonversi tinggi badan cm ke m
		double BMI = bb / (konversi * konversi); //menggunakan ekspresi aritmatika
		//menggunakan if else agar hasil bmi sesuai degan kriteria
		String kategori; if (BMI < 18.5 ) { 
			kategori = "kurus";
		}else if (BMI < 24.9) {
			kategori = "normal";
		}else if (BMI < 29.9) {
			kategori = "gemuk";
		}else if (BMI >= 29.9){
			kategori = "obesitas";
		}else {
			kategori = "tidak normal"; //jika hasil <18,5 
		}
		String hasil = "Berat Badan: " + bb + "kg" + "\nTinggi Badan: " + TB + "cm" + "\nNilai BMI: " + BMI + "\nKategori: " + kategori;
		
		JOptionPane.showMessageDialog(null, hasil, "hasil perhitungan BMI anda:", JOptionPane.INFORMATION_MESSAGE);
	}

}


```

---

## 🔍 Hasil Uji Coba

###  🔢 input

<img width="1920" height="1080" alt="Screenshot 2025-11-09 135228" src="https://github.com/user-attachments/assets/9e491528-2869-43a3-9071-e651df41f1c4" />

### 📊 Output

<img width="1920" height="1080" alt="Screenshot 2025-11-09 135256" src="https://github.com/user-attachments/assets/87fcff46-334a-454d-a050-2d4fb34480c9" />


---

## ✅ Kesimpulan
Program berhasil dijalankan dan menampilkan hasil bmi dengan benar.  

---
