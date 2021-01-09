## Git : Versiyon Kontrol Sistemi

##### Başlangıç ayarları

Bilgisayarımıza git yükledikten sonra config ayarlarını yapmalıyız.

`git config --global user.name="Berke Karataş"`

`git config --global user.email="uberke.karatas@gmail.com"`

Yaptığımız değişiklikleri görmek için **--list** komutunu kullanmalıyız.

`git config --list`

____

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

____

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

Örneğin, VSCode'u açalım ve index.htmlde yaptığımız değişikliklere bakalım(index.htmlde değişiklik yapıp *git add index.html* dediğimizi varsayıyorum). Sonrasında bu kodu(*git restore index.html*) yazdığımız zaman, add işleminden önceki index.html durumu nasılsa kodlarımız o ana geri dönecektir.

___