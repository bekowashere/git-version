## Git : Versiyon Kontrol Sistemi

##### Başlangıç ayarları

Bilgisayarımıza git yükledikten sonra config ayarlarını yapmalıyız.

`git config --global user.name="Berke Karataş"`

`git config --global user.email="uberke.karatas@gmail.com"`

Yaptığımız değişiklikleri görmek için **--list** komutunu kullanmalıyız.

`git config --list`

___

Klasörümüzün içinde **Git Bash** çalıştırdıktan sonra sırasıyla yazmamız gereken komutlar :

`git init`

**.git** klasörü oluşturur, boş bir git reposu - *localrepo*

`git status`

Hangi **branch**da olduğumuzu söyler ve dosyaların durumunu gösterir. *Untracked files* yani daha eklemeyen dosyaları kırmızı olarak gösterir.

`git status -s`

Status özet, short form.

`git add <filename>`

Tekli olarak eklemek istediğimiz dosyayı eklememizi sağlar.


`git add .`
`git add --all`
`git add -A`

Bütün dosyaları eklememizi sağlar.

___

`touch text.txt`

**touch** komutu dosya oluşturmamızı sağlar.

`rm text.txt`

**rm** komutu seçilen dosyayı silmemizi(remove) sağlar

`ls -al`

Linux'daki **ls** komutunun, Windows'daki **dir** komutunun aynısı. Dosyaları listeler.

`mv text.txt readme.txt`

Dosya adını değiştirmemizi sağlar.

___

Bazen yaptığımız dosyaları geri almak isteyebiliriz. **Commit** işleminden önce işlemlerimizi geri almak için aşağıdaki komutlarını kullanmalıyız.

`git restore --staged <filename>`

Bu işlemi yaptıktan sonra **git status** yaparsak file'mız tekrar kırmızı olarak gözükecektir. Yani **staging area**dan **working directory**mize geri döndürür.

Örneğin, *git add index.html* yaptığımızı varsayalım. Bu kodumuzdan sonra *git status* yazarsak git bash komut satırında kırmızı renkte **modified: index.html** yazısını görürüz.

`git restore <file>`

Yaptığımız değişikleri iptal eder, geri alır. 

Örneğin, VSCode'u açalım ve index.htmlde yaptığımız değişikliklere bakalım(index.htmlde değişiklik yapıp *git add index.html* dediğimizi varsayıyorum). Sonrasında bu kodu(*git restore index.html*) yazdığımız zaman, add işleminden önceki index.html durumu nasılsa kodlarımız o ana geri dönecektir bunu anlık olarak VSCode'da gözlemleyebiliriz.

___

##### Commitleri Görmek 

`git show`

Atılan son **commit**i gösterir.

`git log`

**Detaylı** olarak bütün commitleri gösterir. Örnek:

```
commit 5aaefadea5b9a20b80123a7a7f4f18a1d1c9cbb4
Author: Berke Karataş <uberke.karatas@gmail.com>
Date:   Sat Jan 9 04:41:44 2021 +0300

restore

```

`git log --oneline`

Attığımız commitlerin ilk 7 hanesini ve commitini gösterir.

**5aaefad birinci kısım tamamlandı**

`git log -p -2`

Atılan son 2 commiti gösterir

`git log --since=30minutes`
`git log --since=5hours`
`git log --since=3days`
`git log --since=2weeks`

Belirlediğimiz zaman aralığında atılan commitleri gösterir. 
