<h1 align="center"> Hetzner Kullanımı </h1>

<h1 align="center"> Peki neden Hetzner? </h1>

```
# Daha önce neden hetzner kullandığımı ve sunucu kıyaslaması yapmıştım, dolayısıyla özet geçeceğim. 
 
> Hetzner VPSde de, VDS'de de en ucuzu.
>> Bugün 2 CPU 2 RAM andromeda kurdum 3$'a, farklı firmalardan almak istesem 13-18$ arası ödemek durumundayım.
>>> Lokasyon tercihlerinde ek ücret yok, setup fee yok. (kurulum ücreti genelde 5-7 dolardır)
>>>> Referansla üye olduysanız 20$ hediye veriyor ve istediğiniz zaman istediğiniz kadar sunucuda kullanabiliyorsunuz.
>>>>> Yeni kullanıcının test etmesi ve emin olması için 20$ hele ki Türk insanına bal gibidir.

> Hetzner VPS'ler arasında en verimlisi hele de fiyatının ucuzluğuna rağmen. Herhangi bir node patlaması veya benzeri bir şey yaşamadım.
>> Sunucu satın aldığınızda sunucu aktifken işletim sistemi değiştirebiliyorsunuz (data gider)
>>> Sunucu satın aldığınızda 48 saat içersinde sunucu elinize ulaşacak diye bir şey yok, anında veriliyor. (Şu an 10 sunucum var)

> Arayüz kullanımı çok kolay, sunuculara isim verme, sunucuyu resetleme, şifre değiştirme, snapshot alma, IP değişme, çok kolay.
>> Bunları kısaca aşağıda anlatacağım.

> Ve hayat kurtaran kullandıkça ödeme, saatlik ücret ve paranın boşa gitmesi yok.
>> Hetznerde bir sunucu aldınız, bir süre kullandınız, kapattınız ücret yok (veya bir kaç cent)
>>> Sunucu aldınız, ödeme yapmıyorsunuz, kullanıyorsunuz, 1 ay sonra (genellikle ayın 1'i ve 3'ü arası) ödeme istiyor.
>>>> Sunucu iadesi diye bir şey yok, işini bitti mi, delete tuşuna basıp kapatıyorsunuz, ne kadar kullandıysanız alıyor sadece. Bazende almıyorlar düşük kullanımda.

> Daha fazla özellik olabilir aklıma gelmiyor, iyi veya kötü yanlarını eklemek isteyen pull request yapabilir.

# Kötü yanları:

> Hetzner ödeme vb. konularda bu kadar kolaylık sağladığı için haliyle KYC mevcut.
>>> Sanırım her sanal kartı kullanamıyoruz, ödeme konusunda visa istiyor, kaydı kaydederken insanı kanser edebiliyor.
>> Kripto para ile ödeme yok.
>> Hetzner'de referans paylaşabilmek için belli miktar para harcamak veya zaman harcamak gerekiyor.
```

<h1 align="center"> Nasıl kullanılabilir? </h1>

> Hetzner'in 20 dolar bakiyesini almak isteyenlere [link](https://hetzner.cloud/?ref=PAWOkFS595H5)

```
> Öncelikle, hetznerin  bir çok subdomain'i var haliyle bir çok servisi var. VDS, VPS, cloud servis, storage vs vs..
>> VPS'ler için bu linkten ve arayüzde hetzneri kullanmalısınız: https://console.hetzner.cloud/projects
```

![image](https://github.com/ruesandora/Hetzner/assets/101149671/51ab9fa6-6c23-43fb-82f0-0b94827ef3ff)

<h1 align="center"> Adım adım anlatım </h1>

```
> New Project kısmından eğer yeni bir proje ise yeni bir alan açıyorum.
>> Daha sonra Sağ üstten add server diyerek serverimizi oluşturmaya başlıyoruz.
```
![image](https://github.com/ruesandora/Hetzner/assets/101149671/ebf828b7-23c3-423d-8fe9-e285e5372015)

```
> Lokasyon seçiyoruz.
>> Tecrübeyle sabit, Alman sunucuları en iyi çalışanlar.
>>> Bir işletim sistemi seçiyoruz, genelde Ubuntu 20.04 tercihimdir, en stabil çalışan budur.
>>>> Daha sonra sunucu seçiyorum, genellikle 3 ila 7 dolarlık sunucular tercihimdir.
>>>>> Sunucu tercihi tamamen oluşturacağınız projeye bağlı.
>>>>>> Son olarak da en alttan server name'i proje ismi yapıp sağ taraftan Create&Buy now diyerek sunucumu oluşturuyorum.
>>>> Bir kaç tuşta oluşuyor.
```

<h1 align="center"> En güzel kısım </h1>

> Burada her bir özelliğe bir numara verdim, no-1, no-2.. diye, görselden bakarak hetzneri tam olarak öğrenebilirsiniz.

``` 
# No-1, Burada Hetzner IPv4 ve IPv6 adreslerimiz yazar. SSH bağlantısı (sunucuya bağlanma) yaparken IPv4 (1. olan) kullanırız.
# No-2, Sunucuyu açtığından beri ne kadar tutmuş ve kapatırsan ne kadar ödeyeceğin yazar. Misal benimki $0.30 tutmuş şu an.
# No-3, Sunucuyu komple kapatma, delete derken sunucunun ismini yazıp delete yapıyorsunuz.
# No-4, Rescue, sık kullanırım (unuttuğum için), sunucuya bağlanamadığımda şifreyi değişirm. Burada root password diyerek şifre değiştiriyoruz.
# No-5, Rescale, sunucuyu yükseltmek istediğinizde kullanabileceğiniz alan. (kötü taraf düşürme yok)
# No-6, Rebuild, Sunucunuzu işletim sitemini değiştirmek istediğinizde kulalnabilirsiniz. Mesela ubuntu 18'den 20'ye çıkarmak gibi. (data gider)
# No-7, Buradan direkt sunucunuza SSH bağlantısı yapabilirsiniz, bunuda putty mutty uğraştırdıgı zman kullanırım.
# No-8, Sunucuyu silceksiniz veya reset atacaksınız snapshot almak istersenz buradan alabilirsiniz.
```

![Hetzner anlatım](https://github.com/ruesandora/Hetzner/assets/101149671/2e592842-9178-47f4-8c14-dcb0bb9ebfd3)

> No-9'u ayrı olarak paylaşmak istedim, altta ki görselde ki gibi sunucunuz hakkında veri alabilirsiniz.

> Bazı projeler bu veriyi istiyor, oldukça güzel.

![image](https://github.com/ruesandora/Hetzner/assets/101149671/1ec09ac1-9653-4b07-8c94-c4b5c381cae7)
















