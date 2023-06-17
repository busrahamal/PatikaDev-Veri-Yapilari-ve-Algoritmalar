# Proje 3

## Binary Search Tree

## Soru

**[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]** dizisinin Binary-Search-Tree aşamalarını yazınız.

**Örnek:** root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

## Cevap

***Binary Search Tree Algoritması,*** bir kök (root) olarak belirlenmiş olan sayının, sol tarafına kendisinden küçük değerler, sağ tarafına ise kendinden büyük değerler yazılması sonucunda bir düğümün oluşturulması mantığına dayanan algoritmadır.

### Aşamalar

1- İlk olarak ilk elemanımız olan 7'yi kök (root) olarak belirliyoruz. 

2- İkinci eleman olan 5 sayısını, 7'den küçük olduğu için 7'nin sol alt tarafına yazıyoruz.

                 7
                /
               5

3- Üçüncü eleman olan 1 sayısını, hem 7'den hem de 5'ten küçük olduğu için 5'in sol alt tarafına yazıyoruz.

                 7
                /
               5
              /
             1

4- Dördüncü eleman olan 8 sayısını, root sayımız olan 7'den büyük olduğu için 7'nin sağ alt tarafına yazıyoruz.

                 7
                / \ 
               5   8
              /
             1

5- Beşinci eleman olan 3 sayısını, 1'den büyük ve 5'ten küçük olduğu için ve de 5'in sol alt tarafına yazamayacağımız için 1'in sağ alt tarafına yazıyoruz.

                 7
                / \ 
               5   8
              /
             1
              \
               3

6- Altıncı eleman olan 6 sayısını, 7'den küçük ve 5'ten büyük olduğu için ve de 7'nin sol alt tarafına yazamayacağımız için 5'in sağ alt tarafına yazıyoruz.

                 7
                / \ 
               5   8
              / \
             1   6
              \
               3

7- Yedinci eleman olan 0 sayısını, 1'den küçük olduğu için 1'in sol alt tarafına yazıyoruz.

                 7
                / \ 
               5   8
              / \
             1   6
            / \
           0   3

8- Sekizinci eleman olan 9 sayısını, hem 7'den hem de 8'den büyük olduğu için 8'in sağ alt tarafına yazıyoruz.

                 7
                / \ 
               5   8
              / \   \
             1   6   9
            / \
           0   3

9- Dokuzuncu eleman olan 4 sayısını, 3'ten büyük ve 5'ten küçük olduğu için ve de 5'in sol alt tarafına yazamayacağımız için 3'ün sağ alt tarafına yazıyoruz. 

                 7
                / \ 
               5   8
              / \   \
             1   6   9
            / \
           0   3
                \
                 4

10- Onuncu elemanımız olan 2 sayısını, 1'den büyük ve 3'ten küçük olduğu için ve de 1'in sağ alt tarafına yazamayacağımız için 3'ün sol alt tarafına yazıyoruz. 

                 7
                / \ 
               5   8
              / \   \
             1   6   9
            / \
           0   3
              / \
             2   4

Gerçekleştirilen aşamalar sonucunda ortaya çıkan Binary Search Tree şu şekilde olacaktır:

                 7
                / \ 
               5   8
              / \   \
             1   6   9
            / \
           0   3
              / \
             2   4



