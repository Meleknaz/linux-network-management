# linux-network-management

Linux Ağ Yönetimi Final Projesi
Kişisel Bilgisayarınızda Virtualbox üzerinde 

Ubuntu Desktop 18 veya 20 yükleyin. hostname-bilgisayar ismini uPC1 olarak isimlendirin. Kullanıcı adı olarak soyadınızı seçin.
TinyCore Linux (DCore Linux) Yükleyin. hostname-bilgisayar ismini DC1 olarak isimlendirin. Kullanıcı adı olarak isminizi seçin. 
ubuntu 18 veya 20 Server yükleyin. hostname-bilgisayar ismini userver1 olarak isimlendirin. Kullanıcı adı olarak soyadınızı seçin.
Birbirine bağlantılı Klonlama (Çoğalt) yaparak her birisinden iki tane daha klon üretin.

Klonladıktan sonra bilgisayarların isimlerini uPC2,uPC3, DC2, DC3, userver2, userver3 olarak değiştirin.

Senaryo 1: 

Ubuntu Desktop için Ağ bağdaştırıcı ayarlarını NAT olarak ayarlayıp HOST (Kullandığınız) bilgisayardan SSH bağlantısı yapabildiğinizi (PORT yönlendirme ayarlarını yaptıktan sonra), ping yapamadığınızı gösterin. HOST bilgisayardaki dosya ismi soyadiniz.txt şeklinde olan bir dosyayı misafir (guest) işletim sistemine Misafir eklentileri yükledikten sonra kopyala yapıştır yaparak gerçekleştiriniz.
Dcore işletim sisteminin ağ bağdaştırıcı ayarlarını Köprü bağdaştırıcı olarak seçtikten sonra DC1 IP adresini bulun. SSH bağlantısı yapabilmeniz için gerekli yüklemeleri yaptıktan sonra HOST (Kullandığınız) bilgisayardan SSH bağlantısı ve ping yapamadığınızı gösterin. 
Ubuntu Server için yanlızca anamakine bağdaştırıcısı olarak ayarlama yaptıktan sonra IP adresini bulun. SSH bağlantısı yapabilmeniz için gerekli yüklemeleri yaptıktan sonra HOST (Kullandığınız) bilgisayardan SSH bağlantısı ve ping yapamadığınızı gösterin. 


Senaryo 2: 

Numaranızın son iki rakamı S ve R olarak kabul edilmiştir. 

userver1, userver2 ve userver3 için ağ bağdaştırıcı ayarlarını dahili ağ olarak ayarlayın. Bilgisayarların IP adreslerini statik olarak aşağıda verilen şekilde ayarlayın : 

userver1 : 192.168.R.S

userver2 : 192.168.R.S+1

userver3 : 192.168.R.S+2
Bu üç bilgisayardan birbirilerine ssh yapabildiğinizi ama HOST bilgisayardan bunlara SSH yapamadığınızı gösterin.  ping komutunu kullanarak bu bilgisayarlar arasında haberleşmelerin olduğunu gösterin.
userver1 bilgisayardaki dosya ismi adiniz.txt, soyadiniz.txt ve numaraniz.txt şeklinde olan bir dosyaları userver2 bilgisayarına gönderiniz. Gönderim işlemi için sFTP veya SCP protokolünü kullanmanız gerekir.



Senaryo 3: 

uPC1 , uPC2 , userver1 ve userver2 için bir ağ bağdaştırıcısını NAT, diğerini dahili ağ olarak ayarlayın.

uPC1 ve userver1 dahili ağ ismini dahili1, 

uPC2 ve userver2 dahili ağ ismini dahili2 olarak ayarlayın.

userver1 ve userver2 için üçüncü bir ağ bağdaştırıcısını yine dahili3 olarak dahili ağ olarak ayarlayın.

uPC1 üzerinden veri paketlerinin userver1, userver2 ve uPC2 bilgisayarlarına ayrı ayrı nasıl gittiğini gösteriniz. Bunun için uygun bir komut kullanmanızı gerekiyor. 

