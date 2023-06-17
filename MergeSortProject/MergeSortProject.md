# Proje 2

## Merge Sort
**[16, 21, 11, 8, 12, 22]**

### 1. Soru

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

### Cevap

***Merge Sort,*** dizideki verileri, tek eleman kalacak şekilde küçük parçalara ayırma, o küçük parçaları kendi aralarında küçükten büyüğe doğru sıralama, daha sonra o küçük parçalardaki elemanları, her bir parçadaki eleman ile karşılaştırarak bir araya getirme ve bu şekilde dizi verilerini küçükten büyüğe doğru dizme mantığı kullanan bir sıralama algoritmasıdır.

#### Aşamalar


##### Bölme Aşaması

1- İlk olarak diziyi iki grup olacak şekilde bölüyoruz.

***Önce =*** **[16, 21, 11, 8, 12, 22]**

***Sonra =*** **[16, 21, 11] - [8, 12, 22]**


2- Daha sonra tek eleman kalacak şekilde ilk olarak sol taraftaki elemanları ayırıyoruz.

***Önce =*** **[16, 21, 11] - [8, 12, 22]**

***Sonra =*** **[16] [21, 11] - [8] [12, 22]**


3- Şimdi de ikili olarak kalan kısımların sol tarafındaki elemanları ayırıyoruz.

***Önce =*** **[16] [21, 11] - [8] [12, 22]**

***Sonra =*** **[16] [21] [11] - [8] [12] [22]**


Elemanların tek kaldığını görüyoruz ve burada bölme aşamasını bitirip, birleştirme aşamasına geçiyoruz.

--------------------------

##### Birleştirme Aşaması

Dizimizi bölme aşamasında tek eleman kalacak şekilde ayırmıştık. Şimdi ise aynı mantıkla birleştirme işlemi gerçekleştireceğiz.

1- İlk olarak sol taraftaki eleman ayrı kalacak şekilde diğer iki eleman arasında karşılaştırma yapıyoruz,onları küçükten büyüğe doğru sıralıyoruz ve birleştiriyoruz.

***Önce =*** **[16] [21] [11] - [8] [12] [22]**

***Sonra =*** **[16] [11, 21] - [8] [12, 22]**



2- Şimdi sol tarafta tek olarak bulunan değerimizle oluşturduğumuz ikili değer arasında karşılaştırma yapıyoruz ve küçükten büyüğe doğru olacak şekilde üçlü değerler oluşturuyoruz.

***Önce =*** **[16] [11, 21] - [8] [12, 22]**

***Sonra =*** **[11, 16, 21] - [8, 12, 22]**


3- Son olarak da oluşturduğumuz bu üçlü değerleri soldan başlayarak her bir elemanla karşılaştırıyoruz ve en küçük olanı en sola yazacak şekilde birleştiriyoruz.


* İlk olarak 11 küçük mü 8'den diye bakıyoruz. Hayır cevabını aldığımız için 8'i en sola alıyoruz. 

  ***Önce =*** **[11, 16, 21] - [8, 12, 22]**

  ***Sonra =*** **[8, 16, 21] - [11, 12, 22]**


* Daha sonra 8'i diğer iki değer olan 12 ve 22 ile karşılaştırıyoruz. 12 ve 22, 8'den büyük olduğu için 8 ile işimiz bitiyor ve hiçbir işlem yapmadan bir sonraki değer olan 16 ile karşılaştırma işlemine geçiyoruz.

* Burada 16 sayısı ile 11, 12 ve 22 değerlerini karşılaştırıyoruz. 16 sayısı 11'den büyük olduğu için, 11'i 8'in yanına alıyoruz ve 16'yı da 11'in yerine alıyoruz.

  ***Önce =*** **[8, 16, 21] - [11, 12, 22]**

  ***Sonra =*** **[8, 11, 21] - [16, 12, 22]**


* Daha sonra 11'i diğer iki değer olan 12 ve 22 ile karşılaştırıyoruz. 12 ve 22, 11'den büyük olduğu için 11 ile işimiz bitiyor ve hiçbir işlem yapmadan bir sonraki değer olan 21 ile karşılaştırma işlemine geçiyoruz.


* Burada 21 sayısı ile 16, 12 ve 22 değerlerini karşılaştırıyoruz. 21 sayısı 16'dan büyük olduğu için, 16'yı 11'in yanına alıyoruz ve 21'i de 16'nın yerine alıyoruz.

  ***Önce =*** **[8, 11, 21] - [16, 12, 22]**

  ***Sonra =*** **[8, 11, 16] - [21, 12, 22]**


* İlk sayı dizimizde üçüncü değerimiz 16 olduğu için, 16 sayısını 21, 12 ve 22 sayıları ile karşılaştırıyoruz. 16 sayısı 21 sayısından küçük olduğu için dizimiz aynı kalıyor. 

  **[8, 11, 16] - [21, 12, 22]**



* 16 sayısı 12 sayısından büyük olduğu için 16 ile 12'yi yer değiştiriyoruz. 12 sayısını 11 sayısının yanına, 16 sayısını da 21 ile 22 sayısının arasına alıyoruz. 

  ***Önce =*** **[8, 11, 16] - [21, 12, 22]**

  ***Sonra =*** **[8, 11, 12] - [21, 16, 22]**



* İlk sayı dizimizde küçükten büyüğe doğru sıralama işlemi tamamlandığı için ikinci sayı dizimizdeki değerleri birbirleriyle karşılaştırarak küçükten büyüğe doğru dizme işlemi yapıyoruz.

* Burada ilk olarak 21 sayısını 16 ve 22 sayısı ile karşılaştırıyoruz. 16 sayısı 21 sayısından küçük olduğu için 21 sayısının yerine 16, 16 sayısının yerine 21 yazıyoruz.

  ***Önce =*** **[8, 11, 12] - [21, 16, 22]**

  ***Sonra =*** **[8, 11, 12] - [16, 21, 22]**



* Daha sonra 16 sayısının 21 ve 22 sayısından küçük olduğunu gördüğümüz için 16 sayısıyla işimiz bitiyor. 21 sayısına bakıyoruz. 21 sayısı da 22 sayısından küçük olduğu için ve de 22 sayısını da kıyaslayacağımız bir sayı kalmadığı için algoritmamız burada sona eriyor ve dizimizin son hali bu şekli alıyor: **[8, 11, 12] - [16, 21, 22]** Bunları da birleştirdiğimizde **[8, 11, 12, 16, 21, 22]** dizisini elde etmiş oluyoruz.



---------------------------------------------------------------------------------------------------------------

### 2. Soru

Big-O gösterimini yazınız.

### Cevap

Merge Sort Algoritması'nın Big-O Gösterimi, **O(nlogn)**'dir.