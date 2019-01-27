# Ödeme Formu Tasarımı — 2

Türkiye ve dünyadan ödeme formu örneklerini paylaştığım ilk yazıya [buradan ](oedeme-formu-tasarimi-1.md)ulaşabilirsiniz.

Bu yazıda, bazı ödeme formu tasarım pratikleri için, ödeme formlarını birbirleri ile karşılaştıracağım ve popüler firmaların kullandığını bazı tercihlere değineceğim. Okumayı zorlaştırmamak adına çok fazla görsel kullanmadım. Büyük firmaların ödeme formlarına göz atmak isterseniz ilk yazıya da bakamanızı öneririm.

![](https://cdn-images-1.medium.com/max/800/1*Id95ZSy5XRv3cHWJ4xaFYQ.jpeg)

Hep aklıma takılan, önce kart ismi mi yazılmalı yoksa kart numarası mı sorusu için ödeme formlarına bakarak başlamak istiyorum.

### **Hangisi Önce; kart üzerindeki isim mi kart numarası mı?**

Türkiye ve dünyadaki ödeme formlarının birçoğunda önce kart numarası alınıyor fakat Amazon ve Netflix önce isim bilgisini sormayı tercih ediyor.

![Amazon &#xD6;deme Formu](https://cdn-images-1.medium.com/max/800/1*pIQEV2s1srdnSMfR9Sfgag.png)

Diğer taraftan aslında dünyadaki birçok popüler ödeme formunda kart üzerindeki isim bilgisinin hiç talep edilmediğini görebiliriz.

### **Kart üzerindeki isim gerekli mi değil mi ?**

Apple, Facebook, Stripe, Klarna ödeme formlarında kart üzerindeki isim bilgisi bulunmazken, AliExpres, Amazon, Netflix, Shopify, Google ödeme formlarında kart üzerindeki isim bilgisi mevcut. 

![Klarna &#xD6;deme Formu](https://cdn-images-1.medium.com/max/800/1*_wEB3OpmWVmDQXhbNO6AIA.png)

Aslında burada Google’ı biraz daha ayrı bir yere koyabiliriz, çünkü üye ismini, ödeme formundaki “kart sahibinin adı” bölümüne varsayılan olarak set ediyor.

bu noktada google ve facebook’u kıyaslamak istiyorum ama öncelikle kart üzerindeki ismin önemine dair bir not eklemeliyim.

Kart üzerindeki isim, ödeme işleminde banka tarafından kontrol edilen bir bilgi olmadığı için \(istisnaları mevcut\) dummy bir değer göndermek ödemenin başarısız olmasına sebep olmuyor fakat bu bilgi fraud işlemlerin belirlenmesinde çok kritik. Özellikle chargeback riski yüksek olan sektörlerde şüpheli işlemleri engellemek için kart üzerindeki isimin alınması mecburi olacaktır.

### **Google ödeme formu vs Facebook ödeme formu**

Google ve Facebook; müşteri kitleleri birbirinin aynı \(tüm dünyadan reklam verenler\) olan iki dev şirket.

Göze çarpan belirgin fark, facebook ödeme formunda kart üzerindeki isim bilgisi bulunmazken, Google’da bulunuyor ama o da otomatik olarak set edilmiş olarak ödeme formunu açıyor.

![Facebook vs Google](https://cdn-images-1.medium.com/max/800/1*VMkq-xQE7ziqR_xeidf1Ig.png)

Bu ikisini birbiri ile kıyaslamak yerine, Google, Facebook bir kenera diğerlerini bir kenara koyarak kıyaslamak daha kolay olacak.

### **Google — Facebook vs Diğerleri**

İkisi de dünyanın büyük çoğunluğundan farklı olarak kart saklamayı zorunlu tutuyor. Müşterileri kurumsal ve eticaret dünyası hakkında bilinçli olduğu için, kart saklamayı zorunlu kılmak ödeme yapacak kitleyi negatif etkilemiyor.

> > In Amazon We Trust

bireysel müşterilerde, kart saklamayı zorunlu tutmanın, insanların ödeme sayfasını terk etmesine sebep olduğu kabul görmüş olsa da Amazon’un da kart saklamayı mecbur tuttuğunu unutmamak gerekir. Tabiki burada Amazon’un imajı etkili.

Türkiye’de, iş modeli abonelik üzerine kurulu olmadığı halde ödeme anında kart saklamayı zorunlu tutan bir firma bilmiyorum.

### **Amazon**

Amazondan bahsederken unutmamak gereken bir nokta da güvenlik kodu \(cvv\) almaması. Saklı kartla ödeme yaparken güvenlik kodu kullanılmıyor. Buna rağmen Google ve Facebook ödeme formlarında güvenlik kodu bilgisi var.

Amazon’un dünyanın çoğundan farklı olarak seçtiği tasarım özellikleri bu kadar değil.

Kart ismi, kart numarası, son kullanma tarihi alanları, ödeme butonu çoğunlukla alt alta iken, Amazon tek satır \(yan yana\) diyebileceğimiz bir form kullanıyor. Bu tasarımı tercih ederken sayfanın geri kalanı ile uyumunu dikkate aldığı muhakkak.

### **Son Kullanma tarihi**

Amazon’un dünyadaki örneklerinden farklılaştığı Son bir örnek de son kullanma tarihi girme yöntemi.   
Amazon ödeme formunda son kullanma tarihi, açılır liste \(dropdown list\) ile seçiliyor. Google, Facebook, Apple, Netflix, AliExpress, Stripe, Shopify hep son kullanma tarihinin direk girildiği yöntemi seçmiş.

![Netflix &#xD6;deme Formu](https://cdn-images-1.medium.com/max/800/1*KVQZZZRuDl5_RyWb6crxIw.png)

İlginçtir ki, Türkiye’de neredeyse herkes Amazon’u örnek almış. Hepsiburada, N11, Gittigidiyor, Tsoft, Thy, Yemeksepeti, Trendyol, Kitapyurdu da Amazon gibi, açılır liste ile son kullanma tarihinin seçilmesini tercih ediyor.

![Yemeksepeti &#xD6;deme Formu](https://cdn-images-1.medium.com/max/800/1*4MSMUjIz3hbXNmlOO-epvw.png)

Amazon’u bir de büyük rakibi AliExpress ile kıyaslayalım;

### **AliExpress —kart networkü logoları**

AliExpress ödeme formunda, diğer birçoğundan farklı olarak kart üzerindeki isim bilgisini, son kullanma tarihi ve güvenlik kodundan sonra alınıyor. Ayrıca dünyanın çoğundan farklı olarak ad ve soyad için iki farklı kutucuk kullanmış.

![Aliexpres &#xD6;deme Formu](https://cdn-images-1.medium.com/max/800/1*F4u6PZaRHez5D1E1tfl45g.png)

Ayrıca AliExpress, kabul edilen kart logoları için diğer örneklere göre çok daha fazla logo eklemiş. Genel olarak sadece Master, Visa, Amex logoları tercih edilmesine rağmen AliExpress bunların arasına “Visa Electron”, “Maestro” gibi logoları da eklemiş. THY ödeme formunda da çok sayıda logo var. Bu logoların bilgilendirici özelliğinin ötesinde, ödeme yapacak kişi gözünde güven verdiğine dair bir kanı mevcut. Sanırım burada hedef kitle bu kararda etkileyici.

![](https://cdn-images-1.medium.com/max/800/1*pvzaW35uXj-eorwcxKqtVg.png)

Sadece logolar için değil, tasarımın her alanında hedef kitle çok önemli. Ödeme yapan kişiler arasında farklı profil grupları var ise, her gruba farklı bir tasarım sunabilmek ise bu işin en yüksek seviyesi. Bu konuya sonraki yazılarda tekrar değinmek istiyorum \(Şu an ben de o seviyede değilim :\)

### **Apple ve ödemeyi iki karta bölmek**

Apple online dünyada istisna olan bir yöntemi, tutarı iki farklı karta bölerek tek seferde ödeme yapabilmeyi sunuyor.

![Apple &#xD6;deme Formu](https://cdn-images-1.medium.com/max/800/1*LMoRWFB71h93dTH0iy3ubw.png)

Sepet tutarının yüksek olduğu işimlerde bu yöntem müşteri için avantaj sağlayabilir ama sağladığı avantajların yanında getireceği olumsuz etkiler olacaktır. Bu olumsuz etkiler sadece sepet dönüşüm oranı ile alakalı da değil. Destek ekibine çok sayıda telefon gelmesine de sebep olabilir.

iPod, iPhone, macbook’u yaratan firmanın bir tasarımı hakkında negatif şeyler yazarken insanın eli titriyor ama Google’da “worst apple products ” araması yapınca da ilginç şerlerle karşılaşıyor insan.

### **cvv, cvc, cvc2, cvv2, cid, güvenlik kodu**

Online işlemleri daha güvenli kılmak için, fiziksel ortamdaki kartlı ödemelerdeki “pin” benzeri güvenlik kodu bulunmaktadır.   
bu güvenlik kodu için, Amex, Visa, Master, Discover farklı farklı isimler kullanmakta. Bu sebeple bu farklı kısaltmalar mevcut.   
Peki büyük firmalar ödeme formlarında bu alanı isimlendirirken hangisini tercih ediyor:

**cvc** tercih edenler : Klarna, Google, Stripe, Gittigidiyor, Tsoft , Thy

**cvv** tercih edenler : Apple, Shopify,

**güvenlik kodu** \(security code\) tercih edenler : AliExpress, Facebook, Hepsiburada

Buna ek olarak bu kısaltmalardan biri ve “güvenlik kodu” terimini bir arada kullananlar da var : Yemeksepeti, Trendyol, Netflix,![](https://cdn-images-1.medium.com/max/800/1*k4hdo1oiM0Y-bDrZDHCQBw.png)

### **Ödeme formunun yanındaki kredi kartı resmi**

Başlıkta güzel ifade edemesem de ne demek istediğimi aşağıdaki görsele bakarak görebilirsiniz.

![Gittigidiyor &#xD6;deme Formu](https://cdn-images-1.medium.com/max/800/1*6KT4_Y1RkprIQ6QYqG5zgw.png)

bu yöntem basitliği sağlamak adına dünyada pek tercih edilen bir yöntem değil.  
Türkiye’de ise çok daha sık karşılaşıyorum.

N11, Gittigidiyor, Tsoft bu yöntemi kullanıyor.

### **Bonus: Gabriel Tomescu Ödeme Formu Tasarım Rehberi**

[Gabriel Tomescu](https://uxdesign.cc/@gabrieltomescu) kendi ödeme formu tasarım sürecini [“The Anatomy of a credit card form”](https://uxdesign.cc/the-anatomy-of-a-credit-card-payment-form-32ec0e5708bb) isimli yazısında adım adım, tasarımlarını birbiri ile yan yana görsellerle kıyaslayarak anlatmış.

![Gabriel Tomescu&#x2019;nun kendi &#x15F;irketi The Wave i&#xE7;in tasarlad&#x131;&#x11F;&#x131; &#xF6;deme Formu](https://cdn-images-1.medium.com/max/800/1*eErA6h-Q1cfB-6qBOHL9fQ.png)

E-ticaretin uygulamasının en önemli ve hatta nihai amacı olan ödeme alma adımında, birkaç kutucuktan oluşan formun tasarımında bile bu kadar çok farklılaşmayı görmek, tek bir doğru olmadığını gösteriyor.

Bu çeşitlilikte; iş modeli, sepet ortalaması, yerel farklılıklar, hedef kitle profili ve alışkanlıkları muhakkak çok etkili oluyor.

Bir sonraki yazıda, seçeceğim bir ödeme formu ayrıntılı olarak inceleyeceğim. Özellikle, ilk bakışta göze çarpmayan ama ödeme formu tasarımında çok önemli yeri olan **validasyon**lardan bahsedeceğim.

{% hint style="info" %}
_Ödeme formu tasarımı ve bu yazı hakkındaki soru, yorum ve önerilerinizi benimle paylaşabilirseniz çok memnun olurum._
{% endhint %}

