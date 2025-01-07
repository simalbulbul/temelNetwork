### Ağ Maskesi (Subnet Mask)

Bir ağda cihazların birbirleriyle iletişim kurabilmesi için, her cihazın bir IP adresine sahip olması gerekmektedir. IP adresi, bir cihazı benzersiz şekilde tanımlar ve iki ana kısımdan oluşur: Ağ kısmı ve Host kısmı. Bu iki bölüm, cihazların ait oldukları ağ ile kendilerini tanımalarını sağlar.

Ağ maskesi, IP adresinin ağ kısmını belirleyen bir numaradır ve cihazların hangi ağda olduklarını anlamalarına yardımcı olur. Ağ maskesi sayesinde, bir cihaz, IP adresinin hangi bölümünün ağ bilgisini, hangi bölümünün ise cihaz bilgilerini içerdiğini belirler.

Bu, iki cihazın aynı ağda olup olmadığını belirlemek için oldukça önemlidir. Eğer iki cihazın ağ kısmı aynıysa, bu cihazlar aynı yerel ağda (LAN) bulunuyor demektir. Aksi takdirde, farklı ağlardadırlar.

Bir IP adresine ait network bilgisini bulmak için subnet-mask ile birlikte mantıksal olarak AND'lenir.
Mesela, 123.34.0.1 adresinin ağ maskesi 255.255.0.0 ise, ilgili IP adresin ağ kısmı ve sistem adresi aşağıdaki gibi hesaplanır;

![net12](https://github.com/user-attachments/assets/783fec02-3f2a-49cd-bf53-7474b58879d9)

- Ağ maskesinin yapısı, 255 ve 0 değerlerinden oluşur. 255 değerleri, IP adresinin ağ kısmını temsil ederken, 0 değerleri host kısmını belirtir. Ağ maskesindeki her bir 255, IP adresinin ilgili kısmının ağ adresine ait olduğunu ifade ederken, 0 ise host adresine ait olduğunu gösterir.
- Ağ kısmını belirlemenin temel yöntemi, IP adresi ile subnet maskesi (alt ağ maskesi) arasındaki mantıksal AND işlemi ile yapılır. Mantıksal AND işlemi, her iki bitin aynı olmasına bağlı olarak sonuç üretir. Eğer her iki bit de 1 ise sonuç 1 olur, aksi takdirde sonuç 0 olur.

Daha iyi anlamak için, aşağıdaki örneği ele alalım:

IP Adresi: 123.34.0.1
Ağ Maskesi: 255.255.0.0
IP adresi ve ağ maskesi ikili sistemde şu şekilde görünür:

IP Adresi (ikili): 01111011.00100010.00000000.00000001

Ağ Maskesi (ikili): 11111111.11111111.00000000.00000000

Mantıksal AND işlemi yapıldığında:

01111011 AND 11111111 = 01111011 (123)

00100010 AND 11111111 = 00100010 (34)

00000000 AND 00000000 = 00000000 (0)

00000001 AND 00000000 = 00000000 (0)

Sonuç olarak, ağ adresi 123.34.0.0 elde edilir. Bu, cihazın ait olduğu ağın adresidir.

Ağ maskesi, IP adresinin ağ kısmını tanımlayarak, cihazların hangi ağda bulunduklarını anlamalarına olanak tanır. Bu işlem, ağ yapılandırmalarında ve cihazlar arasında iletişim kurulmasında temel bir rol oynar. Mantıksal AND işlemi ile ağ adresi bulunarak, cihazların aynı ağda olup olmadıkları kolayca belirlenebilir.
