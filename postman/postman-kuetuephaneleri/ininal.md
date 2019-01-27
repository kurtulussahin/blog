# ininal

[ininal](https://medium.com/@ininalkart)’ın geliştiriciler için sunduğu API’ını kolayca inceleyebilmek ve test edebilmek için hazırladığım postman kütüphanesini [bu linkten](https://www.getpostman.com/collections/6dc8437dc3c85e2444b1) indirebilirsiniz: [![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/6dc8437dc3c85e2444b1)

![](https://cdn-images-1.medium.com/max/800/1*hsOuynkRlXjxJxKikNjdyw.png)

Postman kütüphanesini[ ininal resmi API dokümantasyonu](https://developer.ininal.com)na göre hazırladım.

İlk olarak ininal tarafından hazırlanmış [“Nasıl Başlarım”](https://man.ininal.com/docs) dokümanını okumak faydalı olacaktır.

Ardından kütüphaneyi indirip Api ve Secret Key’lerinizi bir environment olarak eklemelisiniz. Developer sayfası üzerinden [kayıt](https://developer.ininal.com/apply) olarak test key’lerine sahip olabilirsiniz.

![](https://cdn-images-1.medium.com/max/800/1*IEzixRujaF4xAfw2Pxex0w.png)

Ardından Access Token servisi çağırılarak belirli bir süre geçerli olacak olan accesstoken bilgisi alınır. ininal API’deki diğer tüm servisler için bu servisten dönen accessToken kullanılacaktır.

![](https://cdn-images-1.medium.com/max/800/1*Admt0BGHmPG49XCHghSR3A.png)

Postman kütüphanesi, accessToken’ı environment değişkenleri içine otomatik olarak eklemektedir. Yani Access Token servisini çağırdıktan sonra, herhangi birşey yapmadan diğer servisleri çağırabilirsiniz. Postman kütüphanesi Authentication için gerekli değişkenleri Pre-request Script’ler ile set edecektir.

![](https://cdn-images-1.medium.com/max/800/1*l0JeCzzHfJlFTs1vvhfWpA.png)

[ininal developer sayfası](https://developer.ininal.com/)nda detaylarından bahsedilen servisleri, kütüphane içindeki klasörlerde bulablirsiniz.

![](https://cdn-images-1.medium.com/max/800/1*8Ge8sI0d1Nkx_HwhytayeA.png)

{% hint style="info" %}
_ininal Api postman kütüphanesi hakkında sorularınız olursa iletişime geçmekten çekinmeyin._
{% endhint %}

