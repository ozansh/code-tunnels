#### Screen Komutu Nedir?
Linux'ta screen komutu, terminalinizi multiplex etmek ve birden çok pencere veya oturumu tek bir terminal penceresi içinde yönetmenizi sağlamak için kullanılır. screen komutu genellikle uzun süren işlemleri yönetmek, uzaktan erişimde bağlantıyı sürdürmek veya birden çok görevi aynı anda çalıştırmak için kullanılır.

Screen komutunu kullanmanın temel bazı örnekler:
1- Yeni bir Screen Oturumu Başlatma:

```bash
screen
```
Bu komutla yeni bir screen oturumu başlatılır.

2- Screen Oturumundan Ayrılma:
Ctrl + A ardından D tuş kombinasyonu ile Screen oturumundan ayrılabilirsiniz.

```bash
Ctrl + A, D
```
3- Çalışan Screen Oturumlarını Listeleme:

```bash
screen -ls
```
4- Varolan Bir Oturuma Yeniden Bağlanma:

```bash
screen -r
```
veya

```bash
screen -r <oturum-id>
screen -ls # ile listelenen oturumların ID'lerini kullanarak belirli bir oturuma bağlanabilirsiniz.
```

5- Yeni Pencere Oluşturma:
Yeni bir pencere oluşturmak için Ctrl + A ardından C tuş kombinasyonunu kullanabilirsiniz.

```bash
Ctrl + A, C
```
6- Penceler Arasında Geçiş Yapma:
Ctrl + A ardından N (sonraki pencere) veya P (önceki pencere) tuş kombinasyonları ile penceler arasında geçiş yapabilirsiniz.

```bash
Ctrl + A, N  # Sonraki pencere
Ctrl + A, P  # Önceki pencere
```

7- İsimli Pencere Oluşturma
```bash
screen -S isim
```

Bu örnekler, screen komutunun temel kullanımlarını içermektedir. screen hakkında daha fazla bilgi için, terminalde şu komutu kullanarak man sayfasını inceleyebilirsiniz:

```bash
man screen
```