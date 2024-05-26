### Code Tunnels Nedir?
Önceki senaryonun ve bu senaryonun asıl amacı size Visual Studio Code Tunnels aracını tanıtmak ve sizi bu aracı kullanabilir hale getirmektir.

VSCode Tunnels (Buradan sonra kısaca Tunnels ya da tunnel şeklinde bahsediceğim) Microsoftun geliştirdiği VSCode CLI aracının bir parçasıdır. Bu araç ile uzaktan eriştiğiniz bir makineye kendi tercihiniz olan VSCode sürümünden erişebilirsiniz.

#### SSH'dan farkı nedir?
SecureSHell kısaca kullanıcılara güvenilir olmayan ağlar üzerinden güvenli bir şekilde uzaktaki bir makineye erişimi sağlayan bir araçtır. Aynı zamanda SSH bir ağ protolüdür ve 22 portundan çalışır. Bu ağ protokolüne ve bu protokolü kullanan temel araçlar bütününe SSH denir.

SSH ile çalışırken bağlanıcağınız makinenin ip'sini bilmeniz gerekmektedir. Aynı zamanda bu aracı kullanırken şifre bazlı ya da anahtar bazlı kimlik doğrulama gereklidir.

Tunnels de ise, Github ya da Microsoft hesabınız ile kimlik doğrulama yapmanız gerekir. Kimlik doğrulamanız bir kez yaptıktan sonra doğrulamayı yaptığınız makine için kalıcı hale gelir ve tunnel aracı çalıştıkça makinenize herhangi bir cihazdan VSCode uygulaması üzerinden erişebilirsiniz. 
#### Kullanım amacı
Sonradan bahsedeceğim kurulum adımlarından sonra, BulutBilişimciler platformu da dahil olmak üzere uzaktan bağlanmak istediğiniz makinelere makinenin ***SSH portu kapalı olsa dahi*** kendi bilgisayarınızdan kendi ayarlarınızla birlikte bağlanabileceksiniz.
#### Online ide'den farkı nedir?
![architecture](./assets/server-arch-latest.png)
Online ide konseptinde görselde gözüken VSCode bloğu da yani idenin kendisi de sunucuda, uzaktan erişilen makinede çalıştırılıyor. Bu da sunucuda çok kaynak tüketimine ve web sayfasında sorunlara yol açıyor. Code server yaklaşımında ise idenin arayüzü, eklentileri ve kısacası uzaktaki makinede tutmak istediğiniz dosyalar dışındaki herşey kullanıcının tercih ettiği platformda saklanıyor. Ki burada kullanıcının kendi alışık olduğu geliştirme ortamı konfigirasyonları olabileceğinden dolayı bu kullanıcı deneyimini geliştirir. 

Ayrıca ek olarak masaüstü VSCodunuzdan doğru sürükle bırak yoluyla kendi ilgisayarınızdan dosya paylaşabilirsiniz uzak makinenize.

#### Peki Nasıl Çalışır?
Aracı uzaktan eriştiğiniz makinada çalıştırdığınızda sırasıyla şu adımlar gerçekleşir;

- Araçı komut satırından çalıştırın

- Araç sizden Microsoft ya da Github hesabınızla kimlik doğrulama aşaması
    - Burada size bir auth-key veriliyor ve siz bu anahtarla tercih ettiğiniz hesabınızla doğrulama yapıyorsunuz. 
- Makineye isim verme aşaması 
    - Burada aracı çalıştırdığınız makineye bir isim veriyorsunuz.
- Araç tamamen ayağa kalkıyor (Burada 5-10 saniye bekleyebilirsiniz)

Sonraki adımda uygulanmasına daha detaylı değineceğim.
