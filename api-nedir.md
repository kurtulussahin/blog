# Hiç Bilmeyenler İçin; API Nedir?

![](https://cdn-images-1.medium.com/max/1600/1*Bdd61bDgoidSbfRhkWCerQ.jpeg)

Yıllar once API’nin ne demek olduğunu öğrenmem gerektiğinde bu konuda internetteki birçok yazıyı okuduğumu fakat tam olarak kafamda canlandıramadığımı hatırlıyorum.

Bu yazıda, en ufak bir fikri olmayanlar için, API’nin ne olduğunu olabildiğince basitleştirilmiş şekilde, bir örnekle anlatmaya çalışacağım.

**Öncelikle API‘den bağımsız sıradan bir dünya ile başlayalım.**  
Twitter’da her gün bir özlü söz paylaştığımız hesabımız olduğunu düşünelim. Ayrıca bu hesap hakkında atılan twitleri\(_mention_\) de yine her gün bilgisayarımızda bir dosyaya kaydettiğimizi hayal edelim.

![](https://cdn-images-1.medium.com/max/1600/1*OdGY_9qiZJycamqpuZZ5Hw.jpeg)

Her gün bir twit atmak için internet tarayıcıda adres bölümüne “[twitter.com](http://twitter.com/)” yazarak giriyoruz, ilgili kutucuğa özlü sözü yazıp “_twitle_” butonuna basıyoruz. Ardından twitin yayınlandığı görülüyor.   
Sonrasında hesabımızın bahsedildiği twitler için arama kutusuna hesap adımızı yazıp hakkımıdaki twitleri listeleyerek kopyalayıp dosyamıza kaydediyoruz.

Buraya kadar yaptığımız işlemlerde, tarayıcı ve twitter firmasının bize sunduğu web sitesini; bu sitedeki twit gönderme ve arama özelliklerini manuel olarak kullandık, klavye, mause ve monitör ile bu özelliklere erişim sağladık.

Peki tüm bu işlemleri, \(her gün bir twit atma, twitleri arama\) tamamiyle otomatik olarak yapsak nasıl olurdu. Bu mümkün müdür?   
[Twitter’ın API’ı](https://developer.twitter.com/) ile mümkün. Twitter, web sitesinde sağladığı özellikleri ve hatta daha fazlasını içeren bir API sunmaktadır.

![](https://cdn-images-1.medium.com/max/1600/1*2zxQEObndIiONcRbzzE2UQ.jpeg)

Bu API ile Twitter’da yapacağınız işlemler bir yazılım ile programlanabilir.  
Sizin için her gün bir twit atacak ve hakkınızda bahsedilen twitleri arayıp kayıt edecek bir uygulama geliştirilebilir.  
Artık API’ın açılımı biraz daha anlamlı gelecektir; **“Uygulama Programlama Arayüzü”**

**Şimdi API’nin olduğu dünyayı hayal edelim.**

Twitter API’si ile, ona sorgu yapması için kodlanan uygulama, önceden hazırlanmış listedeki özlü sözlerden her gün birini bizim için paylaşabilir, ardından hakkımızdaki twitleri arayarak bir dosyaya kaydedebilir. Uygulama çalıştığı surece ek bir manuel işe gerek kalmayacaktır.

![](https://cdn-images-1.medium.com/max/1600/1*YQgjmcd3w_slT5aRGvWLmA.png)

Burada bir API’nin sağladığı önemli bir faydayı görmüş olduk. API’ler _**otomasyon**_ imkanı verir, süreçleri hızlandırmayı, programatikleştirmeyi saglar.

**Aynı örnek ile devam ederek birkaç API teriminin üzerinden geçelim;**

![](https://cdn-images-1.medium.com/max/1600/1*zvoS6xxuaGC0WGZRk7dNKw.jpeg)

**Endpoint \(Sorgu Adresi\):** Twit atarken tarayıcıda _twitter.com_ adresini görürsünüz,  
kodunuz API’a sorgu yaparken _https://api.twitter.com/1.1/statuses/update.json_ **endpointini** kullanır.

**Request \(Sorgu\):** Web sayfasında twit’i yazıp “_twitle_” butonuna basarsınız, API ile twit metnini twit gönderme endpointine bir “sorgu” yaparak iletirsiniz.

**Request Data \(Sorgu verisi\):** Yapılan sorguda gönderilen veri. Örnek bir twit atma sorgusu datası : [_https://api.twitter.com/1.1/statuses/update.json?status=Bu_](https://api.twitter.com/1.1/statuses/update.json?status=Bu)_%20Bir%20Test%20Twittidir._

**Parametre:** API’ye gönderdiğiniz twit metni, bir paramatredir. “status” isimli parametre ile Twit metni iletilir.

**Response \(Sorgu cevabı\):** Web sitesinde, twit yayınlandığında ekranda yazdığınız twit’i en üst sırada görürsünüz. Api’de kod ile kolay anlaşılabilecek şekilde, twit’in yayınlandığı mesajını\(ve daha birçok bilgi\) içeren bir metin döner. Tarayıcılara bu bilgi “html” olarak döner ve taratıcı bu html i bizim gözümüzle incelediğimiz görüntüye dönüştürür. API ise “json” denen metin formatında cevap döner.

**Client/library/sdk \(Kütüphane\):** Yazılımcının API’ye kolaylıkla sorgu yapabilmesi için hazır kodlar/kod kütüphaneleridir.

**Authentication \(Doğrulama\):** Web sitesi sizin kim olduğunuzu girişte sorduğu “kullanıcı adı” ve “şifre” ile bilmektedir. API’lar da benzer şekilde “key”ler kullanır.

## 

**Son olarak farklı birkaç API örneği daha vermek istiyorum;**

**eBay API:** eBay’da satılacak ürünleri tek tek elle girmek yerine, otomatik olarak yükleyebilirsiniz.

**Stripe API:** Web sitenizden yapacağınız satışlarda, kart bilgisi ve ödeme isteği Stripe API’a iletilir.

**AccuWeather API:** Sitenizde veya uygulamanızda hava durumu bilgisi göstermek isterseniz, bilgileri bu API’dan otomatik olarak alabilirsiniz.

## 

![](https://cdn-images-1.medium.com/max/1600/1*Xof70YJQrhCh6kiIxYxVDw.png)

Umarım bu yazı API hakkında aklınızda genel bir fikir oluşmasına yardımcı olmuştur.

API’ler hakkında aklınıza takılan soruları, bu yazı hakkındaki yorumlarınızı ve hatta düzeltmek istediğiniz yanlışlarımı lütfen paylaşmaktan çekinmeyin.

