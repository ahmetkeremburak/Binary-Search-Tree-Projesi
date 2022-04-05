# Binary-Search-Tree-Projesi
patika.dev Veri Yapıları ve Algoritmalar dersinin Binary Search Tree projesi

## Proje

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

## Çözüm

1.	Öncelikle dizimizi sıralı bir hale getiriyoruz.
		
		`[0,1,2,3,4,5,6,7,8,9]`
		
2.  Dizinin ortasındaki elemanı kök olarak alıyoruz. Söz konusu dizide ortada bir eleman yok, 4 veya 5'i alabiliyouz.
    Sol tarafta kökren küçük elemanlar, sağ tarafta kökten büyük elemanlar kalmalı.

    ```
                5
               / \
    [0,1,2,3,4]   [6,7,8,9]
    ```
 3. Aynı işlemi sağda ve solda kalan parçalara da uygulamaya devam ediyoruz.

     ```
                    5
                /        \
               2          7 
              / \        / \
         [0,1]  [3,4]  [6]  [8,9]
         
                     5
                /        \
               2          7 
              / \        / \
             1   3      6   8
            /     \          \
           0       4          9
                      
     ```
