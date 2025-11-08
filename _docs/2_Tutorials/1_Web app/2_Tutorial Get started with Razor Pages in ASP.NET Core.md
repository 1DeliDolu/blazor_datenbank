## 🎬 ASP.NET Core Razor Pages ile Başlarken


---

### 🌐 Giriş

Bu eğitim, **ASP.NET Core Razor Pages** kullanarak sıfırdan bir web uygulaması geliştirmeyi adım adım öğretir.

Razor Pages, ASP.NET Core’un sunduğu modern, basit ve güçlü bir **sayfa tabanlı (page-focused)** web geliştirme modelidir.

> 💡 Bu, Rick Anderson tarafından hazırlanmış serinin  **ilk dersidir** .
>
> Serinin sonunda bir **film veritabanı uygulaması (Movie App)** geliştirmiş olacaksın. 🎞️

---

### 🧩 Razor Pages Nedir?

Razor Pages, ASP.NET Core MVC yapısına benzer ama **daha sade** bir model sunar.

Her “sayfa” kendi C# kodu (`.cshtml.cs`) ve HTML görünümü (`.cshtml`) ile birlikte çalışır.

Bu yaklaşım sayesinde:

* Sayfa tabanlı web siteleri daha kolay inşa edilir,
* Kod ve görünüm bir arada tutulduğu için **bakım ve test süreçleri** daha kolay olur,
* Gereksiz controller karmaşası ortadan kalkar.

---

### 🎯 Bu Eğitimin Amacı

Bu ilk derste öğreneceklerin:

✅ Yeni bir **Razor Pages Web App** projesi oluşturmak

✅ Uygulamayı çalıştırmak

✅ Proje yapısını anlamak

Serinin ilerleyen derslerinde şu konular yer alacak:

* 🧱 Model ekleme (`Movie` sınıfı)
* ⚙️ Razor Pages sayfalarını otomatik oluşturma (Scaffolding)
* 🗄️ Veritabanı bağlantısı kurma (Entity Framework Core)
* 🔍 Arama, filtreleme ve doğrulama (validation) ekleme

---

### 🧰 Ön Bilgiler

Eğitime başlamadan önce aşağıdaki araçların kurulu olması gerekir:

| Araç                                        | Açıklama                                                                                             |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| 🔹**.NET 8 SDK**                       | En güncel .NET sürümü,[Download .NET](https://dotnet.microsoft.com/download)adresinden indirilebilir. |
| 🔹**Visual Studio 2022 / VS Code**     | C# ve web geliştirme desteği etkin olmalı.                                                          |
| 🔹**MS SQL Express (isteğe bağlı)** | Veritabanı örnekleri için.                                                                          |

---

### 🪄 Serinin Amacı

Eğitimin sonunda elinde, **film listesini** yöneten bir web uygulaması olacak:

* 🎬 Filmleri listeleyebilirsin,
* ✏️ Yeni film ekleyebilirsin,
* 🗑️ Mevcut kayıtları silebilir veya güncelleyebilirsin,
* 🔍 Filmler arasında arama yapabilirsin.

Tüm bu işlemler, **Entity Framework Core** ile SQL veritabanına bağlı çalışacak.

---

### 🔗 İleri Düzey Kaynaklar

* [Introduction to Razor Pages](https://learn.microsoft.com/aspnet/core/razor-pages) — Deneyimli geliştiriciler için detaylı açıklama
* 🎥 *Video:* [Entity Framework Core for Beginners](https://learn.microsoft.com/ef/core) — Başlangıç seviyesi için görsel anlatım
* [Choose an ASP.NET Core UI](https://learn.microsoft.com/aspnet/core/fundamentals/choose-ui) — Proje türüne göre UI seçimi

---
