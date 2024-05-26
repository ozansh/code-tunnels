### CLI parametreleri
-- help argümanıyla araç hakkında bilgilendirme alabilirsiniz
```bash
./code --help
```
--version argümanıyla aracın versiyonunu görebilirsiniz
```bash
./code --version
```

#### Tam Kurulu VSCode için bazı örnekler
Argüman olarak bir dizin gönderebilirsiniz, bu şekilde gönderdiğiniz dizinde vscode ekranı açılacaktır. Benzer şekilde ilk argüman olarak bir dosya gönderdiğinizde o dosya VSCode içerisinde açılacaktır. Ancak bu senaryo dahilinde CLI aracını kendi başına indirdiğimizden dolayı bu komutlar çalışmayacaktır.
```bash
# Dizin Açma Örneği
./code /home/bulutbilisimci/workspace

# Dosya Açma Örneği
./code /home/bulutbilisimciler/workspace/turktelekom.config
```
Daha derin okuma için [buraya](https://code.visualstudio.com/docs/editor/command-line) bakabilirsiniz