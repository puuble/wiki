---
title: Varlık Adı Formatı
description: Varlık Adı Formatı Özelleştirme
published: true
date: 2023-03-26T15:47:04.458Z
tags: varlık adı, varlık adı formatı
editor: markdown
dateCreated: 2023-03-26T15:38:19.003Z
---

# Varlık Adı Formatı
> Sipariş geldiğinde siparişe ait Müşteri Varlığının hangi formata oluşturulacağını bu bölümden belirleyebilirsiniz.
{.is-info}

- [:mag: Değişkenler *Varlık adı formatı oluştururken değişken kullanabilirsiniz.*](/sambapos/degiskenler)
{.links-list}

> Aşağıda Örnek Formatları Görebilirsiniz.
{.is-info}

```bash
{musteriAdi}
#Sadece Müşteri Adıyla Varlık Oluşturur. Örn: Mehmet Y.
```

```bash
{musteriAdi} - {musteriTelefon}
#Müşteri Adı - Müşteri Telefonu. Örn: Mehmet Y. - 5321234567
```

```bash
{musteriTelefon}
#Sadece Müşteri Telefonuyla Varlık Oluşturur. Örn: 5321234567
```

```bash
{musteriAdi} - {musteriId}
#Müşteri Adı - Müşteri Benzersiz Kodu. Örn: Mehmet Y. - 08ds9a8d0a0ad8
```

```bash
Getir Müşterisi
#Getir Yemekten Gelen Tüm siparişler için sabit bir varlık kullanabilirsiniz. Bu durumda müşteri adı, adresi, telefonu gibi bilgileri özelleştirme sayfasından etiket olarak eklemeniz gerekir.
```

