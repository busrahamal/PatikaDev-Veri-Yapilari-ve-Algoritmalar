# Proje 2

## Merge Sort
**[16, 21, 11, 8, 12, 22]**

### 1. Soru

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

### Cevap

***Merge Sort,*** dizideki verileri, tek eleman kalacak şekilde küçük parçalara ayırma, o küçük parçaları kendi aralarında küçükten büyüğe doğru sıralama, daha sonra o küçük parçalardaki elemanları, her bir parçadaki eleman ile karşılaştırarak bir araya getirme ve bu şekilde dizi verilerini küçükten büyüğe doğru dizme mantığı kullanan bir sıralama algoritmasıdır.

#### Aşamalar

###### Bölme Aşaması

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





