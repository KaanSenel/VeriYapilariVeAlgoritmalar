# Binary Search Tree

Binary Search Tree (İkili Ağaç Yapısı) node'lardan oluşan , her node'un 2 adet child node'a sahip olduğu veri yapısıdır.
Peki nedir bu node kavramı ?

Node, bir veri yapısının en temel birimidir.
Nodelar veri içerebilir ve birbirleri ile bağlantılıdır.

Bu algoritmada en üstte bulunan node'a **root** adı verilir.

Root değerinden küçük değere sahip olan node'lar root'un sol tarafına yerleşir.

Root değerinden büyük değere sahip olan node'lar root'un sağ tarafına yerleşir.


#### [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamaları

İlk değer olan 7 root seçilir. 5 değeri root değerinden küçük olduğu için sol tarafa yazılır.

![img.png](img.png)

1 değeri 7'den küçüktür, sola tarafa gider, 5'ten de küçüktür o yüzden 5'in sol altına yazılır.

![img.png](images\img2.png)

8 değeri 7'den büyüktür, root'un sağ tarafına yazılır.

![img.png](images\img3.png)

3 değeri 7'den küçüktür, 5'ten küçüktür ama 1'den büyüktür, bu yüzden 1'in sağ tarafına yazılır.

![img.png](images\img4.png)

6 değeri 7'den küçüktür, 5'ten büyüktür, bu yüzden 5'in sağına yazılır.

![img.png](images\img5.png)

0 değeri 7'den, 5'ten ve 1'den küçüktür, bu yüzden 0'ın soluna yazılır.

![img.png](images\img6.png)

9 değeri 7'den ve 8'den büyüktür, bu yüzden 8'in sağına yazılır.

![img.png](images\img7.png)

4 değeri 7'den ve 5'den küçüktür, 1'den ve 3'ten büyüktür, bu yüzden 3'ün sağına yazılır.

![img.png](images\img8.png)

2 değeri 7'den ve 5'den küçüktür, 1'den büyük ama 3'den küçüktür, bu yüzden 3'ün soluna yazılır.

![img.png](images\img9.png)





