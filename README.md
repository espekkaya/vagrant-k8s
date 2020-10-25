# vagrant-k8s

Vagrant ile kubernetes lab ortamı oluşturulmasını sağlamaktadır.

Bilgisayara [virtualbox][1] ve [vagrant][2] kurulu olması gerekmekte.

Daha sonra tek yapmanız gereken vagrant' ı ayağa kaldırmanız

    $ git clone https://github.com/espekkaya/vagrant-k8s.git
    $ cd vagrant-ks8
    $ vagrant up

'vagrant up' komutu çalıştığında ilgili uygulamaları bilgisayarınıza kuracaktır buda internet hızınıza bağlı olarak sürecektir. Sonra standart ayarlarda 1 master 2 worker node' usizin adınıza ayağa kaldıracaktır.

    $ vagrant ssh kmaster
 
Yukarıdaki kod ile de master sunucusuna ssh yapabiliyor olacaksınız.

Ortamı silmek için;

    $ vagrant destroy
  
İndirilmiş olan herşeyi silmek için;

    $ vagrant box list
    $ vagrant remove <SILINECEK_DOSYA_ADI>

VagrantFile vs sh'ların alındığı github projesi [şurasıdır.][3]

[1]: https://www.virtualbox.org/
[2]: https://www.vagrantup.com/downloads
[3]: https://github.com/justmeandopensource/kubernetes
