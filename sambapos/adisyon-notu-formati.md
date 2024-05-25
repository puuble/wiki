---
title: Adisyon Notu Formatı
description: Adisyon Notu formatını aşağıdaki örneklere göre düzenleyebilirsiniz.
published: true
date: 2023-03-26T15:56:56.289Z
tags: adisyon notu, adisyon notu formatı, samba, sambapos adisyon notu
editor: markdown
dateCreated: 2023-03-26T15:48:41.130Z
---

# Adisyon Notu Formatı
> Sipariş geldiğinde siparişe ait Adisyon Notunun hangi formata oluşturulacağını bu bölümden belirleyebilirsiniz.
{.is-info}

- [:mag: Değişkenler *Adisyon Notu formatı oluştururken değişken kullanabilirsiniz.*](/sambapos/degiskenler)
{.links-list}

> Aşağıda Örnek Formatları Görebilirsiniz.
{.is-info}

```bash
{adisyonNotu}{ziliCalma}{servisistenmiyor}{temassizTeslimat}[ - Teslimat Saati: {teslimatZamanı}]
```
> Adisyon notuyla birlikte teslimat saati, zili çalma, servis istenmiyor, temassız teslimat durumu gibi tüm bilgileri adisyon notunda gösterebilirsiniz.


---


```bash
{adisyonNotu}{ziliCalma}{servisistenmiyor}{temassizTeslimat}
```
> Teslimat saatini özelleştirme sayfasından etiket ekleyerek göstermek isterseniz adisyon notunda olmasına gerek yok. Yukardaki formatı kullanabilirsiniz.


---


```bash
{adisyonNotu}
```
>Sadece müşterinin yazdığı not eklenir. Diğer tüm bilgileri özelleştirme kullanarak adisyon etiketlerine işlenmesi gerekir.
