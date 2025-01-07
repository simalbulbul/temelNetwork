### ping

- Ping, bilgisayarlar arasında iletişim kurmanın ve bağlantı problemlerini çözmenin en yaygın yollarından biridir.
- Ping komutu, bir bilgisayarın (örneğin A bilgisayarı) başka bir bilgisayara (B bilgisayarı) bir paket gönderdiği ve bu paketin karşı bilgisayar tarafından geri gönderilmesi işlemini gerçekleştirir. Bu işlem, bilgisayarların birbirlerine ulaşılabilir olduğunu doğrular.
- Eğer A bilgisayarından gönderilen paket B bilgisayarına ulaşır ve B bilgisayarı bu paketi geri gönderirse, bu, iki bilgisayarın bağlantısının sağlıklı olduğu anlamına gelir.
- Eğer ping sonucu başarısız olursa, ağda bir bağlantı sorunu olduğunu anlayabilirsiniz.
- Ping, veri paketlerinin ne kadar sürede gittiğini ve geri döndüğünü ölçer. Bu, ağdaki iletişim hızını gösterir.

![ping-atma-1-1-e1602411451587](https://github.com/user-attachments/assets/a1a0dd93-fe0a-4c0e-9633-e1a23832c1d9)

### tracert

- Gönderdiğiniz paketlerin her bir router (yönlendirici) tarafından nasıl geçtiğini takip eder. Bu sayede, paketlerin hedefe ulaşırken geçtiği yolları ve bu yolların her birindeki yönlendiricilerin (router'ların) adreslerini görebilirsiniz.
- Bir ağdaki her bir yönlendirici (router), paketleri bir sonraki yönlendiriciye veya hedefe iletir. Traceroute komutu, her router'dan geçen paketlerin geriye dönen yanıtlarını toplar ve hangi yönlendiricilerin kullanıldığını belirler.
- Paket, ağda hangi router'lar üzerinden geçtiğini gösterir. Bu, hedefe ulaşana kadar geçen her yönlendiricinin IP adresini listeler. internetin veya ağın nasıl yapılandırıldığını anlamanızı sağlar. Paketlerinizin hangi router'lar üzerinden geçtiğini görürsünüz.
- Her router'dan yanıt alırken geçen süreyi (ms cinsinden) gösterir. Bu, her router'a ulaşmanın ne kadar sürdüğünü belirtir.

![traceroute-columns](https://github.com/user-attachments/assets/c613d34d-9183-4897-a8b7-ef598c701d6b)

### arp -a

- Bilgisayarınızdaki ARP (Address Resolution Protocol) tablosunu görüntülemek için kullanılır. Bu komut, ağınızdaki cihazların IP adreslerine karşılık gelen MAC adreslerini listeleyerek, ağ üzerindeki cihazlarla yapılan iletişimde hangi IP adreslerinin hangi MAC adresleriyle eşlendiğini gösterir. 
- ARP tablosu, daha önce yapılan ARP sorguları sonucu elde edilen IP-MAC eşleşmelerini saklar, bu sayede tekrar aynı cihazla iletişim kurarken broadcast yapmadan doğrudan MAC adresi kullanılarak iletişim sağlanabilir.
- Bu süreç, ağda iletişimin daha hızlı ve verimli olmasını sağlar, çünkü her IP adresine karşılık gelen MAC adresi sadece bir kez öğrenilir ve sonrasında doğrudan kullanılabilir.

![arp-command](https://github.com/user-attachments/assets/6d9503d2-4826-477a-b6c5-c397851a8102)

### Nslookup

- Bir alan adı (domain name) ile ilişkilendirilmiş IP adreslerini sorgulamak için kullanılan bir komuttur. 
- Bu komut, özellikle DNS (Domain Name System) sunucularıyla iletişime geçerek, kullanıcıların girdiği alan adı için karşılık gelen IP adreslerini bulur. Ayrıca, tersine sorgulama yaparak bir IP adresine karşılık gelen alan adını da öğrenmek mümkündür. 
- Ağ bağlantı sorunlarını teşhis etmek, DNS yapılandırmalarını kontrol etmek ve alan adı ile IP adresi arasındaki ilişkiyi doğrulamak için yaygın olarak kullanılır. 

![128](https://github.com/user-attachments/assets/41574d25-87ab-4fb2-9a39-fa6f06b30c8f)


