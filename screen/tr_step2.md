### Screen Ve Code CLI
Burada size Screen aracının kullanımını Code CLI ile göstereceğim
```bash
# İlk Önce bir screen sessionu oluşturuyoruz
screen -s code-cli
```
![1](./assets/1.png)
Ardından programımımızı çalıştırıyoruz
```bash
./code tunnel
```
![2](./assets/2.png)
Tünelimiz çalışmaya başladığına göre bu sessionu bırakabiliriz:
```bash
Ctrl A + D
```
Sessionu Şu Şekilde görebiliriz:

```bash
screen -ls
```
![3](./assets/3.png)