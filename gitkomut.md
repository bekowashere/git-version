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