# Muster-Siniflandirilmasi
RFM kullanilarak yapilmistir

Buradaki çalışmamı özetleyecek olursam:
Müşteri segmentasyon türlerini açıkladım. Daha sonrasında yaptığım araştırmalar
 sonucunda bi türlerden en çok RFM'in kullanıldığını fark ettim ve bunun kullanmamın daha yararlı olacağını düşündüm.
Daha sonrasında buna uygun bir veri seti bulmaya çalıştım
Bulmuş olduğum veri seti ingiltere tabanlı bir online satış firmasının 01/12/2009 ve 09/12/2011 tarihler arasında yapmış olduğu satışları içeren bir veri setidir.
https://archive.ics.uci.edu/ml/datasets/Online+Retail+II
Kod parçasını basitçe anlatmam gerekirse, kod verimizi analiz etmemizi sağlıyor. Analizlerimizi yaptıktan sonra
RFM yöntemi ile müşterilerimizi segmentize ediyor.

Araştırmam sonucu elde ettiğim,

Müşteri segmentasyon modellerini şöyle belirtebilirim:
1. Coğrafi: Müşterilin bulundukları yerlere göre ayırlmasını sağlar.
Böylelikle belirgin yerlere daha müşteriler daha spesifik alış-veriş yapabilirler
ülke
bölge
kasaba
kırsal veya kentsel alan
iklim
kültürel özellikler
ekonomik durum
Bu tip benzer özellikler kullanılabilir

2. Sosyo-demografik
yaş
cinsiyet
uyruk
medeni hal
eğitim
meslek
gelir düzeyi
Bu gibi bilgiler ışığında sınıflandırabiliriz

3. Psikografik
yaşam tarzı
ilgi alanları
değerler
kişisel özellikler
Bu tip öncelikler göz önüne alınabilir

4. Davranışsal:
satın alma motivasyonu
markaya bağlılık 
ürün siparişi için hazırlı olma
tekrarlı satın alımlar
ürün veya servis kullanma sıklığı

5. Yakın zamanda, sıkılık, para akışı (Recency, Frequency, Monetary -> RFM):
Müşterileri tanımlarken markamıza yaptıkları son girişlere, 
satın alma sıklıklarına ve harcadıkları paranın büyüklüğüne göre sınıflandırlabiliriz

6. Değerli müşteri modeli(High-value customer HVCs):
RFM modeline dayanarak, yaptığınız iş veya uğraştığınız sektör fark 
etmeksizin bu değerli müşterilerin nereden geldiklerini, hangi özellikleri paylaştıkları istencektir. 
Böylelikle onları daimi müşteriniz yapabilir ve elde edebilirsiniz.

7. Müşteri durumu:
Müşteri durumundan kasıt aslında müşterinin akitf veya pasif olma durumudur. Bizlerin belirlediği ölçüde
sisteme giriş yapmazlarsa bu müşteriler pasif olarak sınıflandırabiliriz. 



---------



Bir markamız olduğunu varsayarsak
Müşteri segmentlerimiz şu  yönde olmalıdır:
1. En iyi Müşteri:
Bu müşteri tipi markamıza karşı aşırı ilgidirler. Bu müşteriye bir şeyler aldığında bazı ödüller
 verilmesi bahsi geçen müşterinin ilgisinin devam etmesinin sağlamasına olanak tanımaktadır.
 Bu ödüller indirim, kullanıcın ilgisine göre değişebilir

2. Sadık harcayıcı:
En iyi müşteri segmentinde olduğu gibi bu müşteri segmentindeki müşterier markamıza para harcamayı severler. 
Onlara her haracamasında belirli bir puan(derece) verilir ve zamanla bu müşterilerin en iyi müşteri sınıfında
 olması sağlnamış olur

3. Potansyiel sadık:
Başka markalara olan ilgileri artmadan sadık harcayıcı sınıfında olduğu gibi bir puanlama sistemiyle
 bu müşterilerimizin sadık harcayıcılar olmasını sağlayabilirz.

4. Yeni müşteri:
Bu yeni müşteri ile ilgili elimizde fazla veri olmamasından ötürü bir cold-start problemi yaşamamız olası.
 Bu müşteriye önceki satın alma işleminden yola çıkarak ilgisini
 çekebilecek promosyon ya da kampanyalar ile markamıza olan ilgisini artmasını hedefleriz

5. Sadık müşteri:
Bu müşteri tipi adından da anlayabildiğimiz üzere markamıza sadıktır. Bu müşterilerimizin ilgisini ve memnuniyetini
artırmak amacıyla bazı teşvikler verilebilir.

6. uykuya dalacak müşteri:
Bu müşteri aslında markamızdan sıklıkla alış-veriş yapmaktadır normalde. 
Ama her nasılsa bir süredir markamızdan alış-veriş yapmayalı epey bir süre olmuştur.
Bu müşteriyi tekrardan kazanmak adına promosyonlar yapıbilir, 
kampanyalar oluşturulabilir veyahut ürün tanıtımında artışa gidilebilir

7. Kaybedemeyeceğimiz/Kış uykusuna yatmış müşteri:
Bu müşterinin uykuya dalacak müşteriden pek bi farkı yoktur. sadece bu müşteri uykuya dalacak olan 
müşteriden daha uzun süredir markamızdan alış-veriş yapmamıştır. Bu müşteriyi tekrardan kazanmak için 
müşterinin ölçütlerini tekrardan gözden geçirip bunlara göre daha 
doğru promosyon veya ürün tanıtımı yapılmalıdr.

8. Kaybettiğimiz müşteri:
Bu müşteri markamıza olan ilgisini  yitirmiştir, zaten kaybettiğimiz müşteriye tekrardan kazanmak için promosyonlar 
yapmak çok maliyetli olacağından bu müşteri ile yolları ayırmak en matıklı bir hareket olacaktır.

-------------------------------------------------
Kampanya önerme:
Müşterilerimizi kaybetmek istemiyorsak veya bizimle hali hazırda olan bağının kuvvetini artırmak istiyorsak
kendilerinin kullanıcı profili veya firmamızdan aldıkları eşyaların içeriklerinden yola çıkarak
Öneri sistemlerinin aracılığıyla  müşteri segmentlerine belirlediğimiz hususta kampanyalarımızı veya promosyonlarımızı
önerebiliriz.

Kampanya önerme ile ilgili kod ekleyemedim.
