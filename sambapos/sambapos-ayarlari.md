---
title: SambaPOS Ayarları
description: Entegrasyonun Sorunsuz Çalışması İçin Yapılması Gereken Ayarlar
published: true
date: 2023-03-26T16:10:29.370Z
tags: posentegra, sambapos ayarları, sambapos
editor: markdown
dateCreated: 2023-03-26T10:02:56.183Z
---

# SambaPOS Ayarları
###### PosEntegra SambaPOS Entegrasyonlarınıın sorunsuz çalışması için mevcut kurulu SambaPOS üzerinde aşağıdaki ayarların yapılması gerekir.
- <kbd>1.</kbd> *SambaPOS ürünlerinde "0" fiyatlı ürünler olmamalıdır.*
{.links-list}

> Özellikle daha önce başka firmalara ait entegrasyon kullanan restoranlarda bir çok "0" fiyatlı ürünler olabiliyor. Bu ürünlerin fiyatı "1" yapılabilir veya gerçek fiyatları yazılabilir.
{.is-danger}

> "0" fiyatlı bir ürün kalır ve sipariş gelirse eğer sipariş kaç adet olursa olsun adisyona "1" adet eklenecektir. Dolayısıyla sipariş SambaPOS'a yanlış işlenmiş olacaktır.
{.is-warning}

- <kbd>2.</kbd> *Kurallar içinde "Adisyona Sipariş Eklendi" ile ilişkilendirilmiş kurallar varsa eğer ve porsiyon sorma, fiyat değiştirme gibi bir kuralsa aşağıdaki kısıtlanmalar eklenmelidir.*
{.links-list}

![alpemix_fscrq2ml9s.png](/alpemix_fscrq2ml9s.png)

---
```bash
{TICKET STATE:Kaynak}
Eşleşme Yok
Yemek Sepeti | Getir Yemek | Trendyol Yemek | Migros Yemek
```
---
> Bu kısıtlama eklenmediğinde sipariş Yemek Portallarındaki fiyatlarıyla değil SambaPOS daki fiyatlarıyla adisyona eklenir.
{.is-warning}

- <kbd>3.</kbd> *Varlık Ekranınızda siparişin hangi portaldan geldiğini göstermek için aşağıdaki kodu kullanabilirsiniz.*
{.links-list}
```bash
[='{TICKET STATE:Kaynak}'!=''?'<L00><block 1 #{GLOBAL SETTING:{TICKET STATE:Kaynak}renk} center 120><L00><size 18><color white><b>{TICKET STATE:Kaynak}</b></color></size></block>':'<L00><block 1 Yellow center 65><size 17><color black><b>ARAMA</b></color></size></block>']
```
- <kbd>4.</kbd> *Adisyon Fişlerinde siparişin hangi portaldan geldiğini göstermek için adisyon şablonunda göstermek istediğiniz yere aşağıdaki kodu ekleyebilirsiniz.*
{.links-list}
```bash
{TICKET STATE:Kaynak}
```
- <kbd>5.</kbd> *Adisyon Fişlerinde siparişin portaldaki sipariş numarasını göstermek için adisyon şablonunda göstermek istediğiniz yere aşağıdaki kodu ekleyebilirsiniz.*
{.links-list}
```bash
{TICKET TAG:Sipariş No}
```

> Sipariş No gösterebilmek için Entegrasyona ait Özelleştirme sayfasında Sipariş No etiketi ekli olmalıdır. Silinirse bu özellik çalışmaz.
{.is-warning}


- [<kbd>6.</kbd> **Restoran Oluşturma** *sayfasından restorana ait lisans anahtarını alabilirsiniz.*](/sambapos/restoran-olusturma)
{.links-list}