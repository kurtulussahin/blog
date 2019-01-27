# Renk Körlüğü ve Ödeme Formu Tasarımı

Dünya nüfusunun ortalama % 4.5'inin renk körü olduğunu biliyor muydunuz. Erkeklerin %8'i, kadınların %0.5'i renk körü.

![](https://cdn-images-1.medium.com/max/800/1*boMwQRsetkB7CrAvbEUBQQ.png)

Peki “UX/UI first development” mottosuyla tasarladığınız, kurumunuzu temsil eden renk paleti donattığınız sitenizi bu insanlar nasıl görüyor?

Dahası, eğer bu sitede bir ürün satıyorsanız, şık ve “fancy” ödeme formunuzda, öde butonuna bastıktan sonra bir hata almışlar ise bunu anlayabiliyorlar mı?

Dünyanın en popüler ödeme formlarından biri _**Stripe**_’a ait.

[stripe.com/checkout](https://stripe.com/checkout) adresinden canlı olarak inceleyebilir ve test edebilirsiniz.   
Binlerce web sitesinde kullanılan bir ödeme formu.

Bir renk körünün gözünden bu ödeme formundaki bir validasyon hatasını birlikte inceleyelim. Kart numaramın son hanesini yanlış girerek bu hatayı gerçekleştireceğim.

Öncelikle sıradan insanın nasıl gördüğüne bakalım;

**1- Hatadan önce:**

![](https://cdn-images-1.medium.com/max/800/1*Z55DBuIg1WAW6NLGHpdTBQ.png)

**2-Hatadan sonra :**

![](https://cdn-images-1.medium.com/max/800/1*I7y5OGOheg8Sj3bVUzHtew.png)

Ödeme butonuna bastıktan sonra form titredi ve kırmızı işaretle, kart numarasında bir sorun olduğunu bana söyledi.   
Şimdi de bu iki adıma bir renk körünün gözünden bakalım;

**1- Hatadan önce:**

![](https://cdn-images-1.medium.com/max/800/1*RI7ut1qxc9rixOk-pzs2ig.png)

**2- Hatadan sonra:**

![](https://cdn-images-1.medium.com/max/800/1*hBWsFmvUGEUptVPD0OWWqg.png)

Bir renk körünün dünyasında kart numarasının etrafındaki kalın çizgi, orada bir hata olduğu mesajını veriyor mu emin değilim.

Ben bu test için, ve her gün ziyaret ettiğimiz web sitelerinin bir renk körünün gözünden nasıl göründüğünü biraz olsun anlayabilmek için chrome tarayıcıda _**sprectrum**_ isimli eklentiyi kullandım.

Bu konudaki deneyimlerinizi ve bu yazı hakkındaki yorumlarınızı lütfen paylaşmaktan çekinmeyin.

_Araştırma sürecindeki desteklerinden dolayı_ [_Serkan Karaduman_](https://medium.com/@serkankaraduman)_’a çok teşekkürler._

