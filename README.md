# Imbalance & Classification

Sebelum kita bahas klasifikasi lebih lanjut, kita bahas supervised learning sedikit lagi yaa guyss...

Jadi sebelumnya kita sudah paham bahwa `supervised learning` adalah salah satu jenis dari machine learning yang paling umum dan `supervised learning` memiliki ciri dimana setiap data memiliki label / target untuk masing masing data. Istilah lainnya pada supervised learning terdapat `Independent variable` dan juga `dependent variable`.

Apa itu `Independent variable` dan `dependent variable`? `Independent variable` adalah variabel yang dapat di kontrol dalam sebuah eksperimen atau percobaan ilmiah, sedangkan `dependent variable` seperti artinya jadi variabel ini bergantung terhadap variabel yang diujikan dalam hal ini `dependent variable` akan bergantung kepada `independent variable`. Nah sampai sini sudah paham kan apa bedanya `Independent & Dependent Variable`, bagus selanjutnya kita akan mendalami apa itu klasifikasi.

Balik lagi ke klasifikasi, jadi apa sih itu klasifikasi?
Pada Klasifikasi umumnya `Dependent Variable` terbagi menjadi 2 kelas (label / target), yakni kelas Positif dan kelas Negatif. Jadi singaktnya Klasifikasi adalah salah satu teknik yang dilakukan dalam menentukan `dependent variable` akan menjadi kelas mana berdasarkan `independent variable`. 

**Apa aja sih penerapan klasifikasi pada industri?**
- Industri Kesehatan  
    Klasifikasi penyakit jantung (Heart Disease): Memprediksi apakah seorang pasien memiliki potensi terkena penyakit jantung.
- Industri Keuangan (FinTech)  
    Klasifikasi Pinjaman ke bank (bank loan): Memprediksi apakah nasabah mampu membayar pinjaman dengan lancar.
- Industri Manufaktur  
    Klasifikasi kegagalan mesin: Memprediksi kemungkinan kegagalan mesin atau peralatan sebelum terjadi, sehingga dapat mengambil tindakan pencegahan.
- Dan masih banyak lagi



Dalam konteks Klasifikasi, pada kenyataan nya sering kali bermasalah yang disebabkan ketidakseimbangan kelas (Imbalance Data) dalam pemodelan klasifikasi. Hal ini dapat mengakibatkan hasil yang buruk terhadap kelas minoritas yang disebabkan karena model cenderung condong pada kelas mayoritas karena jumlah kelas mayoritas sangat berbeda jauh dengan kelas minoritas.

**Jadi apa sih itu imbalance data?**  
Jadi imbalance data / ketidakseimbangan kelas pada data adalah situsi dimana proporsi kelas yang berbeda atau tidak seimbang, sebagai contoh pada dataset klasifikasi biner dimana kelas positif mewakili hanya 5% dari total sampel sedangkan kelas negatif mewakili 95% dari seluruh total sampel, dengan demikian kita dapat mengatakan bahwa dataset tersebut merupakan data yang tidak seimbang atau imbalance data.


**Terus gimana cara mengatasi hal tersebut sehingga kinerja model kita tetap baik?**  
Ada beberapa cara yang dapat dilakukan untuk mengatasi hal tersebut, seperti oversampling, undersampling, hingga dengan mengatur `class_weight` / bobot kelas pada model yang digunakan. 


Yuk kita bahas satu persatu dengan melakukan eksperimen langsung pada dataset dummy yaitu `bankloan.csv` yang merupakan dataset pinjaman bank untuk memprediksi potensi nasabah dalam membayar pinjaman.
