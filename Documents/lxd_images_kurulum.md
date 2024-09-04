# LXD image listelemek, Uzaktaki image'lar ile çalışmak..

- Yerelde indirilen veya oluşturulan imajları listeler.

```
$ lxc image list
```

- LXD'nin varsayılan imaj sunucusundaki tüm imajları listeler.

```
lxc image list images:
```

- Belirli bir dağıtım veya sürüm listelemek..

```
lxc image list images: ubuntu
```
>[!NOTE]
> Sürümlerin veya dağıtımların isimlendirmeleri değişiklik göstermektedir. Uygun sürüm
> araştırarak bulunabilir.


## LXD Ubuntu 24.04 VM-Container Kurulumu

- Noble Numbat 24.04 LTS sürümü için aşağıdaki komut yazılır. Sürümün varlığı ve adı
kontrol edilir.

```
lxc image list images: ubuntu/noble
```

- Yüklemek için aşağıdaki komut yazılır.
```
lxc launch --vm images:ubuntu/noble/desktop server_name
```

## LXD Debian 12 (bookworm) VM-Container Kurulumu

- Bookworm Debian 12 sürümü için aşağıdaki komut yazılır. Sürüm adı kontrol ve not edilir.

```
lxc image list images: debian/12
```

- Yüklemek için aşağıdaki komut yazılır.

```
lxc launch --vm images:debian/12 server_name
```

## LXD AlmaLinux 9.4 VM-Container Kurulumu

- Alma Linux 9.4 için aşağıdaki komut  yazılır ve adı kontrol edilir.

```
lxc image list images: almalinux/9
```

- Yüklemek için aşağıdaki komut yazılır.

```
lxc launch --vm images:almalinux/9 server_name
```

### LXD Çekirdek sayısı ve Ram miktarı artırma

- Kurulmuş olan bir sunucu veya sanal ortamın ram miktarını artırmak için aşağıdaki
komut yazılır.
```
lxc config set server_name limits.memory 2GB
```
- Çekirdek sayısını artırmak için ise aşağıdaki komut yazılır.

```
lxc config set server_name limits.cpu 4
```

- Config dosyası görüntülemek için aşağıdaki komut yazılır.
```
lxc config show server_name
```

- Konteyner işlemler sonunda yeniden başlatılmalıdır.
```
lxc restart server_name
```

