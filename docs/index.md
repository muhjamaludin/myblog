# Blog Mas Muhjamaludin

catatan dan jurnal dari pembelajaran _programming_-ku.

## Bagaimana men-_deploy_ **Mkdocs** di *Github Pages*

27 August 2023

* membuat repository baru di github
* _push project_ / catatan ke repository github dengan nama _remote_ **origin**
* melakukan deploy ke _branch gh-pages_ menggunakan fitur built in **mkdocs**. Mkdocs akan melakukan _generate_ _static web_ dengan format komponen *[jekyll](https://jekyllrb.com/)*. 
```shell
    $ mkdocs gh-deploy
```
* jika akun github kamu gratis (bukan enterprise), pastikan bahwa repository dalam _visibility_: _**public**_, karena fitur _github pages_ hanya bisa dipakai untuk repository publik atau _Enterprise_.
* pada repository, pergi ke menu
```
  setting > Pages > Build and deployment > Branch > gh-pages > /root > save
```
* situs kamu akan di deploy di `<https://yourname.github.io>/<your-repository>`
* untuk melakukan update script / dokumentasi, kamu bisa melakukan perubahan kemudian 
```
git add
git commit
git push origin main
```
dan lakukan deploy seperti langkah diatas `mkdocs gh-deploy`.