# Insertion Sort

Insertion sort sıralı diziyi her adımda eleman eleman oluşturan bir sıralama algoritmasıdır.
Düzensiz dizi elemanlarını tek tek ele alarak her birini sıralanmış kısmındaki uygun yerine yerleştirme esasına dayanır.

Başta dizinin 2. elemanı seçilir ve öndeki elemanla karşılaştırma yapılır, eğer önündeki elemandan küçükse yer değiştirirler.
Bu işlem sonunda 3. eleman seçilir ve öndeki elemanlarla karşılaştırma yapılır, önündeki elemanlardan küçükse yer değiştirme işlemi yapılır.
Dizinin sonunda gelene kadar bu algoritma mantığı devam eder.

[22,27,16,2,18,6] Bu diziyi insertion sort algoritması ile sıralama işlemi yapacağız.

- Başlangıçta dizinin ikinci elemanı alınır ve en başa gidene kadar karşılaştırma işlemi yapılır.Burada 1 işlem gerçekleşir
        
[22, <span style ="color:red">**27**</span>,16,2,18,8]  --> 2.eleman olan 27 seçildi, öndeki elemansan büyük olduğu için yer değiştirme yapılmadı.

- Şimdi dizinin 3.elemanı seçilir ve önündeki elemanlarla karşılaştırma yapılır.

[22,27,<span style="color:red">**16**</span>,2,18,8] --> 3.eleman olan 16, 2. elemandan küçük yer değiştirme gerçekleşir.

[22,<span style="color:red">**16**</span>,27,2,18,8] --> 16 değeri 2.indexe geldi, önündeki değerden küçük olduğu için tekrar yer değiştirilir.

####[<span style="color:red">**16**</span>,22,27,2,18,8] --> işlemler sonucu bu sıralama oluşur.

- Dizinin 4.elemanı olan **2** seçilir ve karşılaştırma işlemleri yapılır.

[16,22,27,<span style="color:red">**2**</span>,18,8] --> 2 değeri önündeki değerden küçüktür.

[16,22,<span style="color:red">**2**</span>,27,18,8] --> 2 değeri önündeki değerden küçüktür.

[16,<span style="color:red">**2**</span>,22,27,18,8] --> 2 değeri önündeki değerden düşüktür ve başa gelir.

####[<span style="color:red">**2**</span>,16,22,27,18,8] --> işlemler sonucu bu sıralama oluşur.

- Dizinin 5. elemanı olan 18 seçilir ve karşılaştırma işlemi yapılır.

[2,16,22,27,<span style="color:red">**18**</span>,8] --> 18 değeri önündeki değerden küçüktür.

[2,16,22,<span style="color:red">**18**</span>,27,8] --> 18 değeri önündeki değerden küçüktür.

[2,16,<span style="color:red">**18**</span>,22,27,8] --> 18 değeri önündeki değerden büyüktür.

#### [2,16,<span style="color:red">**18**</span>,22,27,8] --> işlemler sonucunda bu sıralama oluşur.

-Son eleman olan 8 değeri seçilir ve karşılaştırma işlemleri yapılır.

[2,16,18,22,27,<span style="color:red">**8**</span>] --> 8 değeri önündeki değerden küçüktür.

[2,16,18,22,<span style="color:red">**8**</span>,27] --> 8 değeri önündeki değerden küçüktür.

[2,16,18,<span style="color:red">**8**</span>,22,27] --> 8 değeri önündeki değerden küçüktür.

[2,16,<span style="color:red">**8**</span>,18,22,27] --> 8 değeri önündeki değerden küçüktür.

[2,<span style="color:red">**8**</span>,16,18,22,27] --> 8 değeri önündeki değerden büyüktür.

####[2,<span style="color:red">**8**</span>,16,18,22,27] --> işlemler sonucunda bu sıralama oluşur ve dizi Insertion Sort Algoritmasına göre sıralanmış olur.


### Big O

Big O gösterimi : (n-1)+(n-2)+(n+3)+...+1 = (n(n-1))/2 = n^2 sonucuna ulaşırız.
 ##### Sonuç : O(n^2)

### Time Complexity

Best Case : Dizinin sıralı olması. **n**

Worst Case : Dizinin tersten sıralı olması : **n^2**

Average Case : Dizinin normal dağılımı : **n^2**

#### Dizi sıralandıktan sonra 18 sayısı dizinin ortalarında olur.Bu sebeple <span style ="color:red">***Average Case***</span> kapsamına girer

-----

####[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımı

1. [7,<span style="color:red">**3**</span>,5,8,2,9,4,15,6] --> 2.eleman olan 3 seçilir ve karşılaştırma yapılır.
2. [3,7,<span style="color:red">**5**</span>,8,2,9,4,15,6] --> 3.eleman olan 5 seçilir ve karşılaştırma yapılır.
3. [3,5,7,<span style="color:red">**8**</span>,2,9,4,15,6] --> 4.eleman olan 8 seçilir ve karşılaştırma yapılır.
4. [3,5,7,8,<span style="color:red">**2**</span>,9,4,15,6] --> 5.eleman olan 2 seçilir ve karşılaştırma yapılır.

####4.adımın sonunda oluşan dizi [2,3,5,7,8,9,4,15,6] olur.
