# Selection Sort Projesi
## Proje 1
### Soru 1

[22,27,16,2,18,6] -> Insertion Sort

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

### Soru 2

Big-O gösterimini yazınız.

### Soru 3

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

Average case: Aradığımız sayının ortada olması
Worst case: Aradığımız sayının sonda olması
Best case: Aradığımız sayının dizinin en başında olması.

[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

### Soru 4
 
[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

### Cevap 1

[22,27,16,2,18,6]

(22 mi küçük 27 mi diye kontrol edilir. Küçük olan solda kalır.)
[22,27,16,2,18,6] 

(27 mi küçük 16 mı diye kontrol edilir. 16 küçük olduğu için bir sola kayar.)
[22,16,27,2,18,6] 

(22 mi küçük 16 mı diye kontrol edilir. 16 olan bir sola daha kayar.)
[16,22,27,2,18,6]

(27 mi küçük 2 mi diye kontrol edilir. 2 küçük olduğu için bir sola kayar.)
[16,22,2,27,18,6]

(22 mi küçük 2 mi diye kontrol edilir. 2 küçük olduğu için bir sola daha kayar.)
[16,2,22,27,18,6]

(16 mı küçük 2 mi diye kontrol edilir. 2 küçük olduğu için bir sola daha kayar.)
[2,16,22,27,18,6]

(27 mi küçük 18 mi diye kontrol edilir. 18 küçük olduğu için bir sola kayar.)
[2,16,22,18,27,6]

(22 mi küçük 18 mi diye kontrol edilir. 18 küçük olduğu için bir sola daha kayar.)
[2,16,18,22,27,6]

(27 mi küçük 6 mı diye kontrol edilir. 6 küçük olduğu için bir sola kayar.)
[2,16,18,22,6,27]

(22 mi küçük 6 mı diye kontrol edilir. 6 küçük olduğu için bir sola daha kayar.)
[2,16,18,6,22,27]

(18 mi küçük 6 mı diye kontrol edilir. 6 küçük olduğu için bir sola daha kayar.)
[2,16,6,18,22,27]

(16 mı küçük 6 mı diye kontrol edilir. 6 küçük olduğu için bir sola daha kayar.)
[2,6,16,18,22,27]

### Cevap 2

En küçük sayıyı en başa yazmak için n tane işlem yapıldı.
2. sayıyı getirmek için (n-1) adet işlem yapılır çünkü en baştaki sayı zaten bulunmuştu.
3. sayıyı getirmek için (n-2) adet işlem yapılır çünkü baştaki iki sayıyı zaten bulmuştuk.

Toplamda işlem sayısı n*(n+1)/2 = (n^2+n)/2
Big-O gösterimi O(n^2)dir.

### Cevap 3

18 sayısı dizi sıralandıktan sonra tam ortada olduğu için "Average Case" olur.

### Cevap 4

[7,3,5,8,2,9,4,15,6]
(En küçük sayı bulunur. 2 en küçük olduğu için en baştaki ile yer değiştirir)

[2,3,5,8,7,9,4,15,6]
(En küçük ikinci sayıyı ararız. 3'ü bulduk ama doğru yerde olduğu için swap yapılmaz.)

[2,3,5,8,7,9,4,15,6]
(Ardından bir büyük olan 4 seçilir ve 5 ile yer değiştirir)

[2,3,4,8,7,9,5,15,6]
(Bir büyük sayı olan 5 seçilir ve 8 ile yer değiştirir)

[2,3,4,5,7,9,8,15,6]
(Bir büyük sayı olan 6 seçilir ve 7 ile yer değiştirir)

[2,3,4,5,6,9,8,15,7]
(Bir büyük sayı olan 7 seçilir ve 9 ile yer değiştirir)

[2,3,4,5,6,7,8,15,9]
(Bir sonraki sayı 8 fakat yeri doğru olduğu için swap yapılmaz)

[2,3,4,5,6,7,8,15,9]
(Sonraki sayımız 9 ve 15 ile yer değiştirir)

[2,3,4,5,6,7,8,9,15]


