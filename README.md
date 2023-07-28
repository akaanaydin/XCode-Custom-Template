# XCode-Custom-Template

Merhaba,

Dosya yapısı bu şekildedir. İndirdiğiniz klasördeki swift dosyalarının içeriklerini istediğiniz gibi değiştirebilirsiniz. Klasör isimlerini veya swift dosyalarının isimlerini değiştirirseniz proje oluştuğunda ilgili dosyalara ulaşamazsınız. Dosya ekleme ve çıkarma işlemini TemplateInfo.plist dosyasından yapmanız gerekmektedir. Bunun nasıl yapıldığına dair detaylı bir yazı yazacağım.

<img width="319" alt="Ekran Resmi 2023-07-28 04 11 14" src="https://github.com/akaanaydin/XCode-Custom-Template/assets/44496296/1497f155-9769-432a-ab6e-0ff03718edd1">

İndirdiğiniz dosyayı /Users/scissors/Library/Developer/Xcode/Templates klasörüne atarsanız Xcode güncellemeleri yüzünden template kaybolmayacaktır.

Xcode'da yeni bir proje oluştururken ekranda aşağı inerek template'e ulaşabilirsiniz.

<img width="732" alt="Ekran Resmi 2023-07-28 04 08 55" src="https://github.com/akaanaydin/XCode-Custom-Template/assets/44496296/3519235a-d8e0-49ac-af11-1fb17e01c48c">

Template'i seçtikten sonra sizden proje ismi ve root view controller class'ı için isim isteyecek. Buraya gireceğiniz isim ile projeyi ayağa kaldırmak için gerekli olan ve navigation controller'a sahip olan ilk view controller'ı oluşturacak.

<img width="732" alt="Ekran Resmi 2023-07-28 04 09 33" src="https://github.com/akaanaydin/XCode-Custom-Template/assets/44496296/68426f30-1325-46a2-ad64-3f8bb12fdfba">

Proje oluşturulduktan sonra Targets > Projeniz > Build Phases > Copy Bundle Resources alanından Info.plist dosyasını silmeniz gerekmektedir. Info.plist dosyasını Support klasörü içine koyulduğu için bunu silmezseniz run alırken hata alacaksınız. Bu sorunun çözümü için çalışıyorum.

<img width="802" alt="Ekran Resmi 2023-07-28 04 10 21" src="https://github.com/akaanaydin/XCode-Custom-Template/assets/44496296/313882b2-f966-4619-a548-3c3bfe1a0b16">
