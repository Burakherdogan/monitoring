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


