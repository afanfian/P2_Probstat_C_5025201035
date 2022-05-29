# P2_Probstat_C_5025201035
| Nama  | NRP |
|:-------------:| :-----:|
| Fian Awamiry Maulana | 5025201035 |
## Soal No 1  
**A**  
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
**B**  
**Jawab**  
```R  
t.test (y , x , paired=TRUE)
```  
**Keterangan**  
Diketahui nilai statistik dari uji 𝑡 (𝑡) adalah 7,6525, sementara nilai 
probabilitas (p-value) adalah 0,00006003 (atau 6.003e-05).  
**Bukti**  
![1b.png](https://drive.google.com/uc?export=view&id=1p6rvkwgxuThpyv1soP1QxVcqkFdtpHFs)
**C**  
**Jawab**  
* Diketahui nilai probabilitas dari uji 𝑡 (p-value) adalah 0,00006003. 
Karena nilai probabilitas tersebut lebih kecil dibandingkan tingkat signifikansi 𝛼 = 0,05, 
maka hipotesis nol ditolak dan hipotesis alternatif diterima. Hal ini berarti terdapat pengaruh 
yang signifikan secara statistika dalam hal jumlah denyut jantung, sebelum dan sesudah 
mengkonsumsi obat 𝐴 pada tingkat signifikansi 5%.
## Soal No 2  
**A**  
**Jawab**  
**B**  
**Jawab**  
```R  
zsum.test(mean.x=23500, sigma.x = 3900, n.x = 100,  
          alternative = "greater", mu = 20000,
          conf.level = 0.95)
```  
**Keterangan**  
**Bukti**  
![2b.png](https://drive.google.com/uc?export=view&id=1dIP2cZrWoj9IEXiLXisHLkVFVIHv1Qag)
**C**  
**Jawab**  
## Soal No 3  
**A**  
**Jawab**  
**B**  
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
**C**  
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
**D**  
**Jawab**  
```R  
qchisq(p = 0.05, df = 2, lower.tail=FALSE)
```  
**Keterangan**  
* Nilai kritikal Adapun untuk mendapatkan nilai kritikal bisa menggunakan ```qchisq``` dengan ```df=2``` sesuai soal sebelumnya.  
**Bukti**  
![3d.png](https://drive.google.com/uc?export=view&id=17xj0zievfeVvG5pVHTsW8_Ao8oT5vlNn)  

**E**  
**Jawab**  
* Teori keputusan merupakan teori formal yang berfungsi untuk pengambilan keputusan di bawah ketidakpastian. Sebagai contoh aksinya adalah : ```({a}_{a∈A})``` dan kemungkinan konsekuensi : ```({c}_{c∈C})``` ```tergantung pada keadaan dan tindakan```. Maka keputusan dapat dibuat dengan melakukan ```t.test```.  

**F**  
**Jawab**  
* Kesimpulan Kesimpulan yang didapatkan yaitu perbedaan rata-rata yang terjadi tidak ada jika dilihat dari uji statistik dan akan ada tetapi tidak signifikan jika dipengaruhi nilai kritikal.  
## Soal No 4  
**A**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**B**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**C**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**D**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**E**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**F**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
## Soal No 5  
**A**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**B**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**C**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**D**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
**E**  
**Jawab**  
```R  

```  
**Keterangan**  
**Bukti**  
