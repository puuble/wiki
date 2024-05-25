---
title: Menü Eşleştirme
description: Yemek Portalı Menüleri ile SambaPOS Menülerinin Eşleştirilmesi
published: true
date: 2023-03-26T14:42:19.184Z
tags: sambapos menü, yemek sepeti menü, getir yemek menü, migros yemek menü, trendyol yemek menü
editor: markdown
dateCreated: 2023-03-26T14:42:16.163Z
---

# Menü Eşleştirme

> Yemek Portallarındaki ürünlere karşılık sambapoda kullanılmasıni istediğimiz ürünleri eşleştirmemiz gerekir.
{.is-info}

![chrome_qzeauek6s5.png](/chrome_qzeauek6s5.png)

> Sağ ütteki butonlar sırasıyla kullılarak menü eşleştirmesi yapılabilir.

### 1. Site Menü Senkronize Et
> Bu butona tıklayarak Yemek Portalındaki Restoran Menüsünü çekebilirsiniz.
{.is-info}

> Yemek Sepeti Entegrasyonunda bu özellik yok. Sizin bize bildirdiğiniz restoran koduna göre size bir excel göndereceğiz import ettiğinizde restoran menüsü oluşacak. Daha sonra bu menüyü export ederek tekrar bize göndereceksiniz.
{.is-danger}


### 2. Sambapos Senkronize Et
> Bu butona tıklayarak SambaPOS daki Restoran Menüsünü çekebilirsiniz.
{.is-info}

> Restoran SambaPOS Menüsünü bir kere çektikten sonra yeni ürün eklenmediği sürece diğer entegrasyonların menü eşleştirmesini yaparken senkronize etmenize gerek yoktur.
{.is-warning}

### 3. Otomatik Eşleştir
> Bu butona tıklayarak SambaPOS daki Restoran Menüsünü ile Yepek Portalının menüsünü otomatik eşleştirebilirsiniz.
{.is-info}

> Eşleştirme büyük küçük harf duyarlı değildir. Örneğin Lahmacun ve LAHMACUN başarılı bir şekilde eşleştirilecektir.
{.is-success}

### 4. Eksik Ürünleri Oluştur
> Bu butona tıklayarak SambaPOS daki Restoran Menüsünü ile Yepek Portalının menüsünün eleştirilmeyen ürünlerini SambaPOS da otomatik oluşturabilirsiniz.
{.is-info}

> Oluşturulan yeni ürünler otomatik eşleştirilecektir.
{.is-success}

> Otomatik eşleştirme kendiliğinden yapılmazsa eğer tekrar Otomatik Eşleştir Butonunu kullanınız.
{.is-warning}

> Ürün isimlerinde virgül "," varsa bu ürün ismi otomatik olarak doğru oluşturulmayacaktır. Bu ürün ismini SambaPOS üzerinde düzelterek Sambapos Senkronize Et butonunu kullanarak güncelleyiniz, sonrasında ister manuel isterseniz otomatik eşleştir butonunu kullanarak eşleştiriniz.
{.is-danger}

> Eşleştirilmeyen ürünler, yemek portalına yeni eklenen ürünler sipariş geldiğinde SambaPOS a otomatik olarak eklenir. Sipariş aksamaz.
{.is-success}

### Eşleştirme Tipi

>Bir ürünü eşleştirirken ürün etiketi veya ürün porsiyonu seçebilirsiniz.
{.is-info}

>Örneğin müşterinizin SambaPOS unda "Fuse Tea" diye bir ürün var ve Şeftali, Karpuz, Limon seçenek olarak giriliyorsa sizde bu şekilde eşleştirme yapabilirsiniz.
Eşleştirme Tipi olarak Ürün Etiketi Seçtikten Sonra Ürün olarak Fuse Tea Seçin Son sütunda bulunan boşluğa ise Şeftali girin.
{.is-success}

![chrome_bsb6ocecwu.png](/chrome_bsb6ocecwu.png)


>Örneğin müşterinizin SambaPOS unda "Fuse Tea" diye bir ürün var ve Şeftali, Karpuz, Limon porsiyon olarak giriliyorsa sizde bu şekilde eşleştirme yapabilirsiniz.
Eşleştirme Tipi olarak Ürün Porsiyonu Seçtikten Sonra Ürün olarak Fuse Tea Seçin Son sütunda bulunan açılır menüde ise Şeftali seçin.
{.is-success}

![chrome_a23z0kxqop.png](/chrome_a23z0kxqop.png)

