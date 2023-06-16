# Proje 1

## Insertion Sort
**[22, 27, 16, 2, 18, 6]**

### 1. Soru

Yukarıda verilen dizinin insertion sort türüne göre aşamalarını yazınız.

### Cevap

***Insertion Sort,*** dizideki verileri küçükten büyüğe doğru sıralamak için kullanılan sıralama algoritmasıdır. 

1- İlk aşamada hiçbir işlem yapmıyoruz sadece dizideki ilk elemanımız olan 22'yi sıraya almış oluyoruz.

**[22, 27, 16, 2, 18, 6]**


2- Bu aşamada 27 sayısını hemen solunda bulunan 22 sayısı ile karşılaştırıyoruz. 22 sayısı 27 sayısından küçük olduğu için aynı şekilde kalıyorlar. 

**[22, 27, 16, 2, 18, 6]**


3- Daha sonra 27 sayısı ile hemen solunda bulunan 16 sayısını karşılaştırıyoruz. 16 sayısı 27 sayısından küçük olduğu için bu iki sayıyı yer değiştiriyoruz. Yani 27 sayısının yerine 16 sayısını, 16 sayısının yerine de 27 sayısını yazıyoruz ve dizimiz aşağıdaki şekli almış oluyor.

***Önce =*** **[22, 27, 16, 2, 18, 6]**

***Sonra =*** **[22, 16, 27, 2, 18, 6]**


 * Dizimiz bu şekli aldıktan sonra 16 sayısı ile hemen solunda bulunan 22 sayısını karşılaştırıyoruz. 16 sayısının 22 sayısından daha küçük olduğu sonucuna vardığımız için 16 sayısı ile 22 sayısını yer değiştiriyoruz. Bu işlemi gerçekleştirdikten sonra dizimiz aşağıdaki şekli almış oluyor. 

***Önce =*** **[22, 16, 27, 2, 18, 6]**

***Sonra =*** **[16, 22, 27, 2, 18, 6]**


* 16 sayısının sol tarafında karşılaştırılacak başka sayı kalmadığından dolayı 4. aşamaya geçiyoruz.


4- Bu aşamada 2 sayısını, solunda bulunan sayılarla sırayla karşılaştırıyoruz. 


* 2 sayısı 27 sayısından küçük olduğu için 2 sayısı ile 27 sayısını yer değiştiriyoruz. 

***Önce =*** **[16, 22, 27, 2, 18, 6]**

***Sonra =*** **[16, 22, 2, 27, 18, 6]**


* 2 sayısını solunda bulunan 22 sayısı ile karşılaştırdığımızda 2 sayısı 22 sayısından küçük olduğundan dolayı 2 sayısı ile 22 sayısını yer değiştiriyoruz.

***Önce =*** **[16, 22, 2, 27, 18, 6]**

***Sonra =*** **[16, 2, 22, 27, 18, 6]**


* 2 sayısını solunda bulunan 16 sayısı ile karşılaştırdığımızda 2 sayısı 16 sayısından küçük olduğundan dolayı 2 sayısı ile 16 sayısını yer değiştiriyoruz.

***Önce =*** **[16, 2, 22, 27, 18, 6]**

***Sonra =*** **[2, 16, 22, 27, 18, 6]**


* 2 sayısının solunda karşılaştırılacak başka bir sayı kalmadığından dolayı 4. aşamamız burada sona eriyor. 5. aşamaya geçiyoruz.


5- Bu aşamada 18 sayısını solunda bulunan sayılarla sırayla karşılaştırıyoruz.


* 18 sayısı hemen solunda bulunan 27 sayısından küçük olduğu için 18 sayısı ile 27 sayısını yer değiştiriyoruz. 

***Önce =*** **[2, 16, 22, 27, 18, 6]**

***Sonra =*** **[2, 16, 22, 18, 27, 6]**


* 18 sayısı hemen solunda bulunan 22 sayısından küçük olduğu için 18 sayısı ile 22 sayısını yer değiştiriyoruz. 

***Önce =*** **[2, 16, 22, 18, 27, 6]**

***Sonra =*** **[2, 16, 18, 22, 27, 6]**


* 18 sayısı hemen solunda bulunan 16 sayısından büyük olduğu için dizimiz bu şekilde kalıyor ve 6. aşamaya geçiyoruz. 


6- Bu aşamada 6 sayısını solunda bulunan sayılarla sırayla karşılaştırıyoruz. 


* 6 sayısı hemen solunda bulunan 27 sayısından küçük olduğu için 6 sayısı ile 27 sayısını yer değiştiriyoruz.

***Önce =*** **[2, 16, 18, 22, 27, 6]**

***Sonra =*** **[2, 16, 18, 22, 6, 27]**


* 6 sayısı hemen solunda bulunan 22 sayısından küçük olduğu için 6 sayısı ile 22 sayısını yer değiştiriyoruz.

***Önce =*** **[2, 16, 18, 22, 6, 27]**

***Sonra =*** **[2, 16, 18, 6, 22, 27]**


* 6 sayısı hemen solunda bulunan 18 sayısından küçük olduğu için 6 sayısı ile 18 sayısını yer değiştiriyoruz.

***Önce =*** **[2, 16, 18, 6, 22, 27]**

***Sonra =*** **[2, 16, 6, 18, 22, 27]**


* 6 sayısı hemen solunda bulunan 16 sayısından küçük olduğu için 6 sayısı ile 16 sayısını yer değiştiriyoruz.

***Önce =*** **[2, 16, 6, 18, 22, 27]**

***Sonra =*** **[2, 6, 16, 18, 22, 27]**


* 6 sayısı hemen solunda bulunan 2 sayısından büyük olduğu için aynı şekilde kalıyorlar. Böylelikle insertion (selection) algoritmamız ile elemanlarımızı küçükten büyüğe doğru sıralama işlemini tamamlamış oluyoruz.

***Son =*** **[2, 6, 16, 18, 22, 27]**

---------------------------------------------------------------------------------------------------------------

### 2. Soru

Big-O gösterimini yazınız.

### Cevap

Insertion Sort algoritmasında en kötü durum (worst case) i düşünürsek, tüm eleman sayımıza **n** dediğimizde, ilk yaptığımız aşamada n'den başlayarak birer birer azalma olacak ve **n + (n-1) + (n-2)..** şeklinde işlem devam edeceği için hesaplama da **n.(n+1)/2** formülüyle gerçekleştirilecektir. 

Formülü uygulamamız sonucunda elde ettiğiniz **n * (n+1)/2** değerinin Big O Notation'ı da **O(n2)** olacaktır.

---------------------------------------------------------------------------------------------------------------

### 3. Soru 

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

1. Average case: Aradığımız sayının ortada olması
2. Worst case: Aradığımız sayının sonda olması
3. Best case: Aradığımız sayının dizinin en başında olması.

### Cevap

Sıralama sonucunda **[2, 6, 16, 18, 22, 27]** şeklinde bir dizi elde ediyoruz. Burada 18 sayısının ortalarda yer aldığını görmekteyiz. Bundan dolayı 18 sayısı, Average case: Aradığımız sayının ortada olması kapsamına girmektedir. 

---------------------------------------------------------------------------------------------------------------

## Selection Sort

### 4. Soru

**[7, 3, 5, 8, 2, 9, 4, 15, 6]** dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

### Cevap

***Selection Sort Algoritması,*** dizide yer alan elemanları tek tek kontrol eder, en küçük olanları en başa getirme temel mantığı ile çalışır.

#### Adımlar


1- İlk olarak diziye bakıyoruz ve dizideki en küçük değerin 2 olduğunu görüyoruz ve 2 sayısını en sola alıyoruz. 2 sayısının yerine de en başta yer alan 7 sayısını getiriyoruz.

***Önce =*** **[7, 3, 5, 8, 2, 9, 4, 15, 6]**

***Sonra =*** **[2, 3, 5, 8, 7, 9, 4, 15, 6]**


2- Diziye tekrar baktığımızda 2 sayısından sonra en küçük değerin 3 olduğunu görmekteyiz. En küçük değer olan 2'den sonra yer aldığı için, bir değişiklik gerçekleştirmiyoruz, dizimiz aynı kalıyor. 

***Önce =*** **[2, 3, 5, 8, 7, 9, 4, 15, 6]**

***Sonra =*** **[2, 3, 5, 8, 7, 9, 4, 15, 6]**


3- Dizide 3'ten sonra en küçük değerin 4 olduğunu görüyoruz. 4'ü 3'ün yanına getiriyoruz. 3'ün yanında yer alan 5 değerini de 4'ün yerine getiriyoruz. 

***Önce =*** **[2, 3, 5, 8, 7, 9, 4, 15, 6]**

***Sonra =*** **[2, 3, 4, 8, 7, 9, 5, 15, 6]**


4- 4'ten sonra en küçük değerin 5 olduğunu görüyoruz. 5'i 4'ün yanına getiriyoruz. 4'ün yanında yer alan 8 değerini de 5'in yerine getiriyoruz.

***Önce =*** **[2, 3, 4, 8, 7, 9, 5, 15, 6]**

***Sonra =*** **[2, 3, 4, 5, 7, 9, 8, 15, 6]**


* Böylelikle 4 adımı tamamlamış bulunuyoruz. 4 adım sonrasında dizimiz bu şekli almış oluyor: **[2, 3, 4, 5, 7, 9, 8, 15, 6]**