# bs-starter-template

Bootstrap kütüphanesinin Sass ile yeniden oluşturulmasını sağlayan template.

Bu kütüphane oluşturulurken öncelikle bilgisayarda node.js yüklü olmalıdır. Bende v24.19.0 sürümü yüklüydü.

Node.js kontrolü için
node -v
komutunu çalıştırabilirsiniz.

Ardından bs-starter-template kalsörü içinde iken
npm init --yes
komutuyla sass projemizin package.json dosyasının oluşmasını sağladık.

Ardından css klasörü, sass kalsörü ve index.html dosyasını bs-starter-template klasörü altında oluşturduk.
sass klasörü içine main.scss, custom sytle yamak için \_style.scss ve bootstrap kütüphanesindeki değişkenleri override edebilmek için de \_bs_overrides.scss dosyalarını oluşturduk.

package.json dosyasında script alanını aşağıdaki gibi değiştirdik.
"scripts": {
"sass": "sass -w sass:css --no-source-map"
},

bootstrap kütüphanesini projeye eklemek için node_modules klasörümüz oluşması gerek.
npm i sass
kodunu çalıştırarak node_modules klasörümüz oluştu.

Bootstrap kütüphanesini projeye dahil etmek için
npm i bootstrap
kodunu kullandık ve en son sürümü indirdik.

Bootstrap-Icons kütüphanesini indirmek için
npm i bottstrap-icons
koduyla en son sürümü indirdik.

main.scss kütüphanesindeki import kodlarını ekledik.
npm run sass
komutuyla projenin çalışmaya başlmasını sağladık.

Bu repository üzerinde node_modules klasörünü göremeyeceksiniz ancak projeyi indirdiğinizde ya da clone komutuyla kendi bilgisyarınıza çektiğinizde node_modules klasörü ve bağlı kütüphanelerin indirilmesi için
npm i
komutunu çalıştırmanız yeterlidir.
