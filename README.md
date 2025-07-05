M adet benzersiz rastgele sayı üretir ve bu sayılarla bir Binary Search Tree (BST) oluşturur.
Kullanıcıdan k ve p değerlerini alır:
Eğer ağaçta k değeri varsa:
p < k ise k değerini k - p olarak günceller.
p >= k ise k değerli düğümü ağaçtan siler ve değeri bir stack'e (yığına) ekler.
Bu işlem ağaç boşalana kadar sürer.
En son, silinen düğüm değerlerini stack üzerinden yazdırır (son giren ilk çıkar mantığıyla).
Hafızayı temizler.
1. Başlangıçta:
M: Ağaçtaki toplam düğüm sayısı.
N: Üretilecek sayıların 1-N aralığı.
Program M adet benzersiz rastgele sayı üretir ve bunları BST’ye ekler.
2. BST Oluşturulması:
insert() fonksiyonu sayesinde sayılar BST kurallarına göre yerleştirilir.
Ağaç inorder() dolaşımı ile küçükten büyüğe sıralı şekilde yazdırılır.
3. Kullanıcı Girdileri:
Program döngüye girer ve her seferinde kullanıcıdan şu iki değer istenir:
k: Ağaçta aranan değer.
p: Güncelleme veya silme eşiği.
updateOrDelete() fonksiyonu:
Eğer k == düğüm.data:
p < k ise: data -= p
p >= k ise: düğüm silinir ve değeri stack[] dizisine eklenir.
Ağaçta k bulunana kadar sol/sağ dallara ilerler.
4. Ağaç Boşalana Kadar:
Kullanıcı k ve p girmeye devam eder. Ağaçta artık düğüm kalmayınca program bu döngüden çıkar.
5. Stack İşlemi:
Silinen düğüm değerleri stack[] içinde tutulur.
Bu değerler, LIFO mantığıyla empty_stack[] dizisine ters çevrilerek yazdırılır.
