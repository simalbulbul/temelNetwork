### Gateway
- Gateway (yönlendirici), iki farklı ağ arasında veri iletimi yapan cihazdır. Örneğin, evinizdeki modem, cihazlarınızın (bilgisayar, telefon) internete bağlanmasını sağlar. Modem, ev ağınız ile internet ağı arasında bir geçiş noktası gibidir.

- Gateway, genellikle farklı ağlar arasındaki iletişimi sağlar. Kendi ağınızda olan cihazlar arasında ARP sorguları yaparak birbirlerinin MAC adreslerini öğrenir ve iletişimi sağlar. Ancak, eğer bir cihaz başka bir ağla (örneğin internetle) iletişim kurmak istiyorsa, o zaman bu cihazın verileri gateway'e yönlendirilir.

- Bir cihazın, başka bir ağla iletişim kurabilmesi için gateway'in IP adresi cihazın ağ ayarlarında belirtilmelidir. Cihazlar, başka bir ağa veri göndermek istediklerinde, veriyi gateway'e yollarlar ve gateway, veriyi doğru ağa yönlendirir.

Diyelim ki evinizde bir modem var ve bu modem, cihazlarınızı internete bağlıyor. Evinizdeki bilgisayarlar kendi ağlarında iletişim kurarken, ARP sorgusu yaparak birbirlerinin adreslerini öğrenir. Ancak internet gibi dış bir ağla iletişim kurmak istediklerinde, bilgisayarların bu isteği modem'e (yani gateway) yönlendirilir.

IP Adresleri ve Maskeler
Router A için: 192.168.55.29/28
Router B için: 192.168.55.132/25
Router C için: 192.168.55.57/27
Bu IP adresleri, farklı ağlar arasında yönlendirme yapacak olan gateway'lere aittir. Bu cihazların her biri, farklı ağlarda bulunuyor ve farklı subnet maskeleri kullanıyor.

/30 Subnet Maskesi
Bir cihazın, sadece başka bir cihazla iletişim kuracağı durumlar için çok küçük ağlar kullanılır. Bu tür ağlar için /30 subnet maskesi kullanılır. /30, 32 bitlik bir IP adresinde sadece 2 cihazın birbirleriyle iletişim kurmasına olanak tanır.

192.168.55.0/30 ve 192.168.55.1/30 IP adresleri arasındaki ağda yalnızca 2 cihaz bulunabilir.
Bu durumda, 192.168.55.0 ve 192.168.55.3 özel adreslerdir ve kullanılamaz, çünkü 0 ağ adresi ve 3 broadcast (yayın) adresidir.
Yani, 192.168.55.1 ve 192.168.55.2 cihazların IP adresleri olabilir.

![hq720](https://github.com/user-attachments/assets/42f714d6-cd0b-4e8d-bed4-390952d73ce5)

