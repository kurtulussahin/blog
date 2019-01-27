# Sorgular

Postman HTTP sorgularını kolaylıkla yapabilmek için kullanıcı dostu bir arayüz sunuyor.

Bir HTTP sorgusunun 4 parçası olan, _**Url**_, _**method**_, _**header**_, _**body**_ için Postman arayüzünü kullanabilirsiniz.

![Postman aray&#xFC;z&#xFC; request b&#xF6;l&#xFC;m&#xFC;](https://cdn-images-1.medium.com/max/1600/1*1SnUwHxte8fi-glZjLvyog.png)

Adres satırına Url’i girdikten sonra, sol taraftaki dropdown menüden methodu değiştirebilirsiniz. _**POST**_, _**GET**_, _**PUT**_, _**DELETE**_ ile birlikte 15'den fazla methodu kullanmak mümkün.

Request body için 4 farklı format seçeneği bulunuyor; _**Form-Data**_, _**urlEncoded**_, _**raw**_ ve _**binary**_.

Gerekli parametreleri girdikten sonra “Send” butonuna basarak sorguyu gerçekleştirebilirsiniz.

Ek olarak sorgudan önce ve sonra scriptler ekleyebilir, bu sayede dinamik request parametreleri oluşturabilir, dönen response’lar için testler hazırlayabilirsiniz.

Sorgu cevabı Postman arayüzünde _**response**_ bölümünde görüntülenecektir.

![Postman aray&#xFC;z&#xFC; response b&#xF6;l&#xFC;m&#xFC;](https://cdn-images-1.medium.com/max/1600/1*RBd76EeX64UX0NVFdxf5NA.png)

Postman _**response**_ görüntüleyici ekranı, bir API response’ndaki _**body**_, _**header**_ve _**status**_ kodunu görmenize yardımcı olur. Bu temel bilgilere ek olarak, _**response time**_, _**response siz**_e, _**cookie**_’leri de Postman arayüzü sayesinde görebilirsiniz.

Tüm sorgularınız _**history**_ bölümünde daha sonra tekrar erişebilmeniz için kayıt oluyor.

![Postman&#x200A;&#x2014;&#x200A;History](https://cdn-images-1.medium.com/max/1600/1*WQqFJqSkaXEX_jdkN_d8pg.png)

Postman hakkındaki temel yazılardan sonra, request’lerle alakalı _**Authorization**_, _**Debug**_, _**Test**_ konularında ayrıntılı yazılar hazırlayacağım.

Postman‘e aşina olmanın en iyi yolu, bir API üzerinde testler yapmak.  
Bunun [usersdemo.herokuapp.com](http://usersdemo.herokuapp.com/) adresinden inceleyebileceğiniz API’ı kullanabilirsiniz.

Bu API için, bir de _**Postman dokümantasyon**_ özelliğini kullanarak [developer sayfası](https://documenter.getpostman.com/view/78530/users-demo-api/RWEiMJHV) hazırladım. Önümüzdeki yazılarda Postman’in dokümantasyon özelliğine de ayrıca değineceğim.

Bir sonraki yazı **Postman kütüphane**leri hakkında olacak. Users Demo API’ı için hazırladığım Postman kütüphanesini [_buradan_](https://www.getpostman.com/collections/de04d62ba2cb2b55c937) indirebilir, temel sorguları kolaylıkla test edebilirsiniz.

