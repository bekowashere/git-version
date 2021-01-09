## Git : Versiyon Kontrol Sistemi

##### Başlangıç ayarları

Bilgisayarımıza git yükledikten sonra config ayarlarını yapmalıyız.

`git config --global user.name="Berke Karataş"`

`git config --global user.email="uberke.karatas@gmail.com"`


<!-- ___________________________ -->

Yaptığımız değişiklikleri görmek için **--list** komutunu kullanmalıyız.

`git config --list`

___

Klasörümüzün içinde **Git Bash** çalıştırdıktan sonra sırasıyla yazmamız gereken komutlar :

`git init`

**.git** klasörü oluşturur, boş bir git reposu - *localrepo*

`git status`

Hangi **branch**da olduğumuzu söyler ve dosyaların durumunu gösterir. *Untracked files* yani daha eklemeyen dosyaları kırmızı olarak gösterir.

`git add <filename>`

Tekli olarak eklemek istediğimiz dosyayı eklememizi sağlar.


`git add .`
`git add --all`
`git add -A`

Bütün dosyaları eklememizi sağlar.