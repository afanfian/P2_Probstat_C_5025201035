# P2_Probstat_C_5025201035
| Nama  | NRP |
|:-------------:| :-----:|
| Fian Awamiry Maulana | 5025201035 |  

**Note: Jika bukti/gambar tidak muncul saat reload, bisa melihat pada folder dokumentasi** 
## Soal No 1  
**A. Kesimpulan Kesimpulan yang didapatkan yaitu perbedaan rata-rata yang terjadi tidak ada jika dilihat dari uji statistik dan akan ada tetapi tidak signifikan jika dipengaruhi nilai kritikal.**  
**Jawab**  
```R  
x <- c(78,75,67,77,70,72,78,74,77)
y <- c(100,95,70,90,90,90,89,90,100)
sd(x-y)
```  
**Keterangan**  
Berdasarkan perhitungan diperoleh nilai standar deviasi dari data selisih pasangan 
pengamatan, yakni = 6,35959468 atau 6,360.  
**Bukti**  
![1a.png](https://drive.google.com/uc?export=view&id=1GhMP5Jr4WfKu0rDjdGynFc7Fv7J5uLrv)
**B. Carilah nilai t (p-value)**  
**Jawab**  
```R  
t.test (y , x , paired=TRUE)
```  
**Keterangan**  
Diketahui nilai statistik dari uji 𝑡 (𝑡) adalah 7,6525, sementara nilai 
probabilitas (p-value) adalah 0,00006003 (atau 6.003e-05).  
**Bukti**  
![1b.png](https://drive.google.com/uc?export=view&id=1p6rvkwgxuThpyv1soP1QxVcqkFdtpHFs)
**C. Tentukanlah apakah terdapat pengaruh yang signifikan secara statistika
dalam hal kadar saturasi oksigen , sebelum dan sesudah melakukan
aktivitas 𝐴 jika diketahui tingkat signifikansi 𝛼 = 5% serta H0 : “tidak ada
pengaruh yang signifikan secara statistika dalam hal kadar saturasi
oksigen , sebelum dan sesudah melakukan aktivitas 𝐴”**  
**Jawab**  
* Diketahui nilai probabilitas dari uji 𝑡 (p-value) adalah 0,00006003. 
Karena nilai probabilitas tersebut lebih kecil dibandingkan tingkat signifikansi 𝛼 = 0,05, 
maka hipotesis nol ditolak dan hipotesis alternatif diterima. Hal ini berarti terdapat pengaruh 
yang signifikan secara statistika dalam hal jumlah denyut jantung, sebelum dan sesudah 
mengkonsumsi obat 𝐴 pada tingkat signifikansi 5%.
## Soal No 2  
**A. Apakah Anda setuju dengan klaim tersebut?**  
**Jawab**  
* Setuju  

**B. Jelaskan maksud dari output yang dihasilkan!**  
**Jawab**  
```R  
zsum.test(mean.x=23500, sigma.x = 3900, n.x = 100,  
          alternative = "greater", mu = 20000,
          conf.level = 0.95)
```  
**Keterangan**  
**Bukti**  
![2b.png](https://drive.google.com/uc?export=view&id=1dIP2cZrWoj9IEXiLXisHLkVFVIHv1Qag)
**C. Buatlah kesimpulan berdasarkan P-Value yang dihasilkan!**  
**Jawab**  
* Kesimpulan yang didapat adalah bahwa mobil dikemudikan rata-rata lebih dari 20.000 kilometer per tahun.  

**Bukti**
![2c.jpg](https://drive.google.com/uc?export=view&id=1AulpLUXyy0YI-ybml67iB966p1XHjJ0W)
## Soal No 3  
**A. H0 dan H1**  
**Jawab**  
![3a.jpg](https://drive.google.com/uc?export=view&id=1B1wDlKeXTSeOqwRPzmAz2Kt7DVs6PX3-)
**B. Hitung Sampel Statistik**  
**Jawab**  
```R  
install.packages("BSDA")
library(BSDA)

tsum.test(mean.x=3.64, s.x = 1.67, n.x = 19, 
          mean.y =2.79 , s.y = 1.32, n.y = 27, 
          alternative = "greater", var.equal = TRUE)
```  
**Keterangan**  
**Bukti**  
![3b.png](https://drive.google.com/uc?export=view&id=1PD4u0iSUk7UqnanVFycZbkDEVnqu1iQm)
**C. Lakukan Uji Statistik (df =2)**  
**Jawab**  
```R  
install.packages("mosaic")
library(mosaic)

plotDist(dist='t', df=2, col="blue")
```  
**Keterangan**  
* Install terlebih dahulu library ```mosaic``` sebagai berikut: ```install.packages("mosaic")```  
* Setelah menginstall library ```mosaic``` definisikan library ```mosaic``` sebagai berikut: ```library(mosaic)```.  
* Lalu masukkan rumus untuk melakukan Uji Statistik (df=2) ```plotDist(dist='t', df=2, col="blue")```  
**Bukti**  
![3c.png](https://drive.google.com/uc?export=view&id=1pMa_2p8tVNns5yzq1DgQMpjciZggp2QB)  

**D. Nilai Kritikal**  
**Jawab**  
```R  
qchisq(p = 0.05, df = 2, lower.tail=FALSE)
```  
**Keterangan**  
* Nilai kritikal Adapun untuk mendapatkan nilai kritikal bisa menggunakan ```qchisq``` dengan ```df=2``` sesuai soal sebelumnya.  
**Bukti**  
![3d.png](https://drive.google.com/uc?export=view&id=17xj0zievfeVvG5pVHTsW8_Ao8oT5vlNn)  

**E. Keputusan**  
**Jawab**  
* Teori keputusan merupakan teori formal yang berfungsi untuk pengambilan keputusan di bawah ketidakpastian. Sebagai contoh aksinya adalah : ```({a}_{a∈A})``` dan kemungkinan konsekuensi : ```({c}_{c∈C})``` ```tergantung pada keadaan dan tindakan```. Maka keputusan dapat dibuat dengan melakukan ```t.test```.  

**F. Kesimpulan**  
**Jawab**  
* Kesimpulan Kesimpulan yang didapatkan yaitu perbedaan rata-rata yang terjadi tidak ada jika dilihat dari uji statistik dan akan ada tetapi tidak signifikan jika dipengaruhi nilai kritikal.  
## Soal No 4  
**A. Buatlah masing masing jenis spesies menjadi 3 subjek "Grup" (grup 1,grup
2,grup 3). Lalu Gambarkan plot kuantil normal untuk setiap kelompok dan
lihat apakah ada outlier utama dalam homogenitas varians.**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**B. Carilah atau periksalah Homogeneity of variances nya , Berapa nilai p yang
didapatkan? , Apa hipotesis dan kesimpulan yang dapat diambil ?**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**C. Untuk uji ANOVA (satu arah), buatlah model linier dengan Panjang versus
Grup dan beri nama model tersebut model 1.**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**D. Dari Hasil Poin C, Berapakah nilai-p ? , Apa yang dapat Anda simpulkan
dari H0?**  
**Jawab** 
**Keterangan**  
**Bukti**  
**E. Verifikasilah jawaban model 1 dengan Post-hoc test Tukey HSD, dari nilai p
yang didapatkan apakah satu jenis kucing lebih panjang dari yang lain? Jelaskan**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**F. Visualisasikan data dengan ggplot2**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
## Soal No 5  
**A. Buatlah plot sederhana untuk visualisasi data**  
**Jawab**  
* Install terlebih dahulu untuk ```multcompView``` nya.  
```R  
install.packages("multcompView")
```  
* Setelah menginstall ```multcompView``` silahkan mengerun beberapa library dibawah ini dan jangan langsung mengeksekusi programnya.  
```R  
library(readr)
library(ggplot2)
library(multcompView)
library(dplyr)
```  
* Selanjutnya membaca file GTL.csv dari documents.  
```R
GTL <- read_csv("GTL.csv")
head(GTL)
```  
* Selanjutnya, kita melakukan observasi pada data.  
```R
str(GTL)
```  
* Yang terakhir, kita melakukan visualisasi menggunakan ```simple plot```.  
```R
qplot(x = Temp, y = Light, geom = "point", data = GTL) +
  facet_grid(.~Glass, labeller = label_both)
```  
**Bukti**  
* Membaca file ```GTL.csv```.  
![5a1.png](https://drive.google.com/uc?export=view&id=1TTL1uX03OMp3RZMWEzBTAtNEq_VLY-YI)  
* Melakukan observasi data.  
![5a2.png](https://drive.google.com/uc?export=view&id=1mbNUIyXoqKQNLhftrqQrxavG-NQwz091)  
* Visualisasi menggunakan ```simple plot```.  
![5a3.png](https://drive.google.com/uc?export=view&id=1UbNYK2cHmzA5tOvtQ_adbY299fqWRX3T)  

**B. Lakukan uji ANOVA dua arah**  
**Jawab**  
* Membuat variabel ```as factor``` sebagai ```ANOVA```  
```R  
GTL$Glass <- as.factor(GTL$Glass)
GTL$Temp_Factor <- as.factor(GTL$Temp)
str(GTL)
```  
* Melakukan ```analisis of variance```:  
```R
anova <- aov(Light ~ Glass*Temp_Factor, data = GTL)
summary(anova)
```  

**Bukti**  
* Membuat variabel ```as factor``` sebagai ```ANOVA```  
![5b1.png](https://drive.google.com/uc?export=view&id=1g-mFWbOwg9P8Ln22AAmD1EBadFdNANgC)  
* Melakukan ```analisis of variance```:  
![5b2.png](https://drive.google.com/uc?export=view&id=1utSEHh_czTGYDe7YfCRhfrHSxGnSI9b8)  

**C. Tampilkan tabel dengan mean dan standar deviasi keluaran cahaya untuk
setiap perlakuan (kombinasi kaca pelat muka dan suhu operasi)**  
**Jawab**  
* Melakukan ```summarise``` dengan menggunakan cara ```group_by``` sesuai dengan mean dan standar deviasi yang berlaku, sebagai berikut:  
```R  
data_summary <- group_by(GTL, Glass, Temp) %>%
  summarise(mean=mean(Light), sd=sd(Light)) %>%
  arrange(desc(mean))
print(data_summary)
```  
**Bukti**  
![5C.png](https://drive.google.com/uc?export=view&id=1qJmRfw8KhR0YTuSEBc0d8qzFk7pGSRkQ)  

**D. Lakukan uji Tukey** 
**Jawab**  
* Menggunakan fungsi ```TukeyHSD``` sebagai berikut:   
```R  
tukey <- TukeyHSD(anova)
print(tukey)
```  
**Keterangan**  
* Menggunakan fungsi ```TukeyHSD``` dan mengeprint ```tukey```.  

**Bukti**  
![5d.png](https://drive.google.com/uc?export=view&id=1xWx9nCvacIXkJkI7bkHGTxJMsRcCeWoa)  

**E. Gunakan compact letter display untuk menunjukkan perbedaan signifikan
antara uji Anova dan uji Tukey**  
**Jawab**  
* Membuat ```compact letter```.  
```R  
tukey.cld <- multcompLetters4(anova, tukey)
print(tukey.cld)
```  
* Menambahkan ```compact letter display``` kedalam tabel dengan menggunakan ```means``` atau rata-rata dan sd.  
```R  
cld <- as.data.frame.list(tukey.cld$`Glass:Temp_Factor`)
data_summary$Tukey <- cld$Letters
print(data_summary)
```  
**Bukti**  
* Membuat ```compact letter```.  
![5e1.png](https://drive.google.com/uc?export=view&id=1DWt7R0NOMNr0_fZmFE9dCxskOIZsjyjl)  
* Menambahkan ```compact letter display```.  
![5e2.png](https://drive.google.com/uc?export=view&id=11rw8u6VBuW4BcXEBJHfcy4mx61GFp1nI)
