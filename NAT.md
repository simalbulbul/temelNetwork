### NAT

- NAT bir ağda bulunan bilgisayarın, kendi ağı dışında başka bir ağa veya İnternete çıkarken farklı bir IP adresi kullanabilmesi için geliştirilmiş bir İnternet protokolüdür. Yani NAT bilgisayarın sahip olduğu IP adresini istenilen başka bir adrese dönüştürür. Bilgisayarlarımızın iç network üzerinde Private IP adresleri kullandığını biliyoruz. İç networkümüzde kullanmamız için ayrılan bu ip adresleri internette kullanılamazlar ve biz de bu ip adresleri ile internete erişemeyiz. Dolayısıyla internet ortamına girerken internet üzerinde yerimizi belli edecek sabit özel bir IP’ye ihtiyacımız var. İnternet ortamında kullanılan IP adreslere public IP adresi demiştik.

- NAT yaparak Private IP’lerimizi Public IP’ye dönüştürüp internete çıkarken isteklerimizin geri dönmesini sağlamış oluruz. Buna en temel örnek evlerimizdeki modemdir. Modemler local IP’lerimizi internete çıkarken servis sağlayıcımızın bize verdiği Public IP’ye dönüştürerek internete çıkmamızı sağlar. 

![nat](https://github.com/user-attachments/assets/22429fb1-86c3-4634-b2a6-8cef95bfde86)
