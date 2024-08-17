# LXD Container nedir? 

Sistem kaynaklarını izole ederek birden fazla Linux işletim sisteminin tek bir ana bilgisayar
üzerinde çalışmasını sağlayan sanallaştırma teknolojisidir. LXC (Linux Containers) üzerine
inşa edilmiş ve kapsayıcı yönetim için geliştirilmiştir.

## Kullanım Alanları:

- Geliştiriciler, farklı yazılım sürümlerini test etmek için ortamlar oluşturabilir.
- Entegrasyon ve dağıtım süreçlerinde LXD container'lar, test ve dağıtım için izole ortamlar
sağlar.

## Avantajları: 
- Sanal makinelerden daha az kaynak kullanır, yalnızca gerekli bileşenleri izole eder.
- Sanal makinelerden daha hızlı başlatılır, servislerin ve uygulamaların hızlıca başlatılmasını
sağlar.
- LXD, container'ların kolayca oluşturulmasını, yönetilmesini ve izlenmesini sağlar.
- Ana makinede yüzlerce container çalıştırabilmeyi sağlar.

### Stateful ve Stateless Kavramları:

- **Stateful:** Uygulama veya servis, çalışma zamanında belirli bir durumu tutar ve bu durum,
servis kapatılıp tekrar başlatılırsa bile korunur.

- **Stateless:** Uygulama veya servis, hiçbir kalıcı durum tutmaz. Her istek bağımsızdır ve
herhangi bir geçmiş durumdan etkilenmez.

> [!NOTE]
> LXD, tam izole sistemler çalıştırmak ve stateful iş yüklerini yönetmek için daha uygundur.



### Snap Paket Yöneticisi Avantajları
- Farklı Linux dağıtımlarında aynı şekilde çalışarak LXD'yi kendi bağımlılıklarıyla paketler
ve uyumluluk sağlar.
- Snap paketleri otomatik güncellenmesi sayesinde LXD son sürüme sahip olur.
- LXD geliştiricileri tarafından önerilmesi ve bu sebeple desteklenen en güncel sürümün
Snap üzerinden elde edilmesidir.

> [!TIP]
> LXD, yalnızca Snap ile yüklenmek zorunda değildir. Başka paket yöneticileri ile yüklenilebilir.

### Snap KURULUM:

- Debian, Ubuntu, Kubuntu, için yazılacak komutlar.
```
sudo apt update
sudo apt install snapd
```
- Versiyon güncellemek için yazılacak komut.
```
sudo snap install snapd
```

