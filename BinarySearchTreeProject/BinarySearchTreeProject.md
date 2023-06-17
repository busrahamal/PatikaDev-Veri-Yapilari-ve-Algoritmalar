# Proje 3

## Binary Search Tree

## Soru

**[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]** dizisinin Binary-Search-Tree aşamalarını yazınız.

**Örnek:** root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

## Cevap

***Binary Search Tree Algoritması,*** bir kök (root) olarak belirlenmiş olan sayının, sol tarafınakendisinden küçük değerler, sağ tarafına ise kendinden büyük değerler yazılması sonucunda bir düğümün oluşturulması mantığına dayanan algoritmadır.

### Aşamalar

1- İlk olarak ilk elemanımız olan 7'yi kök (root) olarak belirliyoruz. 

2- İkinci eleman olan 5 sayısı, 7 sayısından küçük olduğu için, 7'nin sol alt tarafına yazıyoruz.

                 7
                /
               5

3- Üçüncü eleman olan 1 sayısı, hem 7'den hem de 5'ten küçük olduğu için 5'in sol alt tarafına yazıyoruz.

                 7
                /
               5
              /
             1

4- Dördüncü eleman olan 8 sayısı, root sayımız olan 7'den büyük olduğu için onu 7'nin sağ alt tarafına yazıyoruz.

                 7
                / \ 
               5   8
              /
             1

5- Beşinci eleman olan 3 sayısı, 1'den büyük ve 5'ten küçük olduğu için ve de 5'in sol altına yazamayacağımız için 1'in sağ alt tarafına yazıyoruz.

                 7
                / \ 
               5   8
              /
             1
              \
               3

6- Altıncı eleman olan 6 sayısı, 7'den küçük ve 5'ten büyük olduğu için ve de 7'nin sol altına yazamayacağımız için 5'in sağ alt tarafına yazıyoruz.

                 7
                / \ 
               5   8
              / \
             1   6
              \
               3

7- Yedinci eleman olan 0 sayısını 1 sayısından küçük olduğu için 1'in sol alt tarafına yazıyoruz.

                 7
                / \ 
               5   8
              / \
             1   6
            / \
           0   3





