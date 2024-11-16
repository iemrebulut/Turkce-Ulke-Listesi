# Ülkeler Bilgileri API & JSON Veritabanı

Bu proje, ülkelerin Türkçe isimlerini, ülke kodlarını ve ülke telefon kodlarını içeren JSON dosyalarını ve MySQL veritabanı çıktısını sunmaktadır. Veriler, özellikle uluslararası projelerde veya telefon numarası doğrulama sistemlerinde faydalı olabilir.

## İçindekiler

- `countries.json` - Ülkelerin Türkçe isimleri, ülke kodları ve telefon kodlarını içeren JSON dosyası.
- `countries.sql` - MySQL veritabanı çıktısı olarak ülkelere ait verilerin saklandığı SQL dosyası.
  
## Özellikler

- **Ülke Adı (Türkçe)**: Ülkelerin Türkçe isimleri.
- **Ülke Kodu**: ISO 3166-1 standardına uygun ülke kodları.
- **Telefon Kodu**: Her ülkenin uluslararası telefon kodları.

## Kullanım

### JSON Verisi

Veri, `countries.json` dosyasında aşağıdaki gibi bir yapıda sunulmaktadır:

```json
[
  {
    "name": "Türkiye",
    "country_code": "TR",
    "phone_code": "+90"
  },
  {
    "name": "Amerika Birleşik Devletleri",
    "country_code": "US",
    "phone_code": "+1"
  }
]
```

### MySQL Veritabanı
`countries.sql` dosyasını MySQL veritabanınıza import ederek, ülkeler tablosunu oluşturabilirsiniz.

## Kurulum
1. Reponun içeriğini bilgisayarınıza indirin veya kopyalayın.
2. countries.json dosyasını JSON verisi olarak kullanabilirsiniz.
3. countries.sql dosyasını MySQL veritabanınıza import ederek gerekli tabloyu oluşturabilirsiniz:
    - MySQL veritabanınıza giriş yapın.
    - Aşağıdaki komutu kullanarak SQL dosyasını import edin:
    ```
    mysql -u <kullanıcı_adı> -p <veritabanı_adı> < countries.sql
    ```
4. Veritabanınızda ve JSON dosyanızda yer alan ülke bilgilerine erişebilir ve projelerinizde kullanabilirsiniz.

## Katkıda Bulunma
Ülke listesinin güncel olmadığını düşünüyorsanız katkıda bulunabilirsiniz.

