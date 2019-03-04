# Ödeme Formu Tasarımı — Kart Üzerindeki İsim

Bu yazıda online ödeme formlarındaki “kart üzerindeki isim” alanından Türkiye’deki büyük eticaret sitelerinden örnekler vererek bahsedeceğim.

Kartlı ödeme formu için en temel alanlar , kart üzerindeki isim, kart numarası, son kullanma tarihi ve güvenlik kodu \(cvv\).

Bazı eticaret sitelerinde “kart üzerindeki isim” kısmını görmeyebilirsiniz.

Peki isim bilgisi olmadan işlem nasıl başarılı oluyor?

İsim bilgisi tüm dünyada banka tarafında kontrol edilen bir bilgi değil. Bu sayede bu alan olmadan \(veya dummy set edilerek\) işlem yapılabiliyor.

İsim bilgisi almayan eticaret sitelerine örnek olarak Trendyol ve Yemeksepetini gösterebiliriz.

![Trendyol &#xF6;deme formu](https://cdn-images-1.medium.com/max/800/1*9lwG-zjldUcM6kD5hok28w.png)

![Yemeksepeti &#xF6;deme formu](https://cdn-images-1.medium.com/max/800/1*lenadW_W02LRKpUaoe0XGg.png)

İsim bilgisi almamak özellikle ödeme adımını sadeceleştirmek için tercih edilen bir yöntem.   
Ödeme adımı, kullanıcı için ne kadar basit olursa, siparişini vermesi o kadar kolay olacak ve sepet dönüşüm oranını o kadar arttıracaktır.

Diğer taraftan kart üzerindeki isim bilgisi zorunlu değilse ve bu bilgiyi kullanıcıdan istememek süreci kolaylaştırıyor ise neden halen birçok web sitesinde bu alanı doldurması kullanıcıdan isteniyor?  
Öncelikle bu alının zorunlu 2 eticaret sitesi Hepsiburada ve Sahibinden’e bakalım;

![Hepsiburada &#xF6;deme formu](https://cdn-images-1.medium.com/max/800/1*A-lqT-2KPm8i_Sww8nsdyA.png)

![Sahibinden &#xF6;deme formu](https://cdn-images-1.medium.com/max/800/1*-w1RP3rynoZ-o0xXIbbBew.png)

Kart üzerindeki isim bilgisini kullanıcıdan talep etmenin iki avantajı mevcut;   
ilk olarak kullanıcı alışkanlığını bozmamak. Ödeme yapacak kişinin kart bilgilerini girerken kafasında soru işareti yaratmamak.   
Bundan daha önemli kısım ise şüpheli işlemleri engellemek .  
Fiziksel dünyada çalınan kart bilgilerinde çoğunlukla isim bilgisi bulunmuyor. Örneğin bir ATM’de yapılan kopyalama işleminde kötü niyetli kişiler kart numarası, son kullanma tarihi ve güvenlik kodu bilgisini ele geçirirken isim bilgisine ulaşamıyor.   
Online ödeme işlemi sonucunda bankadan dönen cevapta kart üzerindeki isim maskeli olarak dönüyor.  İşyeri site de ödeme formuna girilen isim ile bankadan dönen değeri kıyaslayarak şüpheli işlemleri tespit edebiliyor.

Son kullanıcı gözünden bakarsak, kart üzerindeki isim bilgisini girip girmemek, veya doğru girip girmemek çok kritik değil.   
İşyeri tarafından baktığımızda ise, fraud riski yüksek olan sektörlerde şüpheli işlemleri engellemek için çok faydalı. Fraud riski düşük olan sektörler için, hedef kitlenin kullanıcı alışkanlığı analiz edilerek ödeme formunda bu alanın olup olmamasına karar verilebilir.

## 

_**Bonus:**   
Bu yazıyı beğendiyseniz, ödeme formu tasarımındaki sadelik konusunda_ [_Mustafa Aktaş_](https://medium.com/@mustafa_aktas_)_’ın “_[_Less is more” yazısın_](https://medium.com/@mustafa_aktas_/less-is-more-25a7ab5407a2)_ı muhakkak okumanızı tavsiye ederim._

_Mustafa Bey’in yazısında özellikle “3ds/güvenli ödeme” seçeneği hakkındaki yorumlarını okuduktan sonra, yukarıda örnek verdiğim sitelerin ödeme formlarında bu seçeneğin kullanıcıya sunulup sunulmadığını kontrol edebilirsiniz._

## 

_Ödeme formu tasarımı ve bu yazı hakkındaki soru, yorum ve önerilerinizi benimle paylaşabilirseniz çok memnun olurum._

_Ödeme formu tasarımı hakkındaki diğer yazılarım;_ 

{% page-ref page="oedeme-formu-tasarimi-1.md" %}

{% page-ref page="oedeme-formu-tasarimi-2.md" %}

{% page-ref page="renk-koerluegue-ve-oedeme-formu-tasarimi.md" %}

