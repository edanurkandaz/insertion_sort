# insertion_sort
www.patika.dev

INSERTION SORT: diziyi küçükten büyüğe sıralamamıza yardımcı olur. İlk önce küçük elemanı aramaya başlarız bulunca dizinin başına atarak 
ya da olması gereken yere atarak devam ederiz. Birlikte inceleyelim.

elimizdeki dizi [22,27,16,2,18,6] olsun.

Bu diziyi INSERTION SORT ile düzenlemek istersek aşağıdaki adımları kullanırız.

1.ADIM:
22 ile 27 kıyasladığımızda 22 nin doğru yerde oldugunu görürüz sıra 16 sayısına geçer ve 27 den büyük olduğu için öne atarız aynı çekilde 22 den de büyük olduğu için en başa gelir. Yani son durumda dizi aşağıdaki gibi olur.
[16,22,27,2,18,6]

2.ADIM:
ilk 3 sayıyı zaten incelemiştik. sıra 2 ye geldi o da hepsinden küçük olduğu için başa alınacak ve dizinin son durumu aşağıdaki gibi olacaktır.
[2,16,22,27,18,6]

3.ADIJM:
sırada 18 var o da 16 ile 22 arasında olduğu için bu aralığa yerleşmesi gerekiyor. Son durumda aşağıdaki dizi meydana gelir.
[2,16,18,22,27,6]

4.ADIM:
Bu adımda ise son sayımız olan 6 ya bakıyoruz. Onun yeride de 2 ile 16 arasında olduğu için oraya alıp insertion sort u bitiriyoruz.
[2,6,16,18,22,27]

Karmaşıklığına bakacak olursak;
Yazdığımız kod içinde ilk olarak bir sayıyı arıyoruz ve bu sayıyı diğer bir sayıyla karşılaştırma işlevi yazıyoruz. Bunun sonucunda yazdığımız kod n^2 nin katı olarak dönüyor. O yüzden bu sıralamamızın karmaşıklığına O(n^2) diyebiliriz.

Time Complexity: 
Average case: Aradığımız sayının ortada olması
Worst case: Aradığımız sayının sonda olması
Best case: Aradığımız sayının dizinin en başında olması

Aradığımız sayıyı 18 olarak varsayarsak dizi sıralandıktan sonra bu sayının ortalarda bir yerde konumlandığını görebiliriz. Yani bizim dizimize average case dememiz doğru bir ifade olacaktır.

Örnek olarak başka bir diziye bakmak istersek; [7,3,5,8,2,9,4,15,6]

bu dizideki adımlar şu şekilde olacaktır.
1--> [3,7,5,8,2,9,4,15,6]
2--> [3,5,7,8,2,9,4,15,6]
3--> [2,3,5,7,8,9,4,15,6]
4--> [2,3,4,5,7,8,9,15,6]
.
.
.
seklinde devam edecektir.
