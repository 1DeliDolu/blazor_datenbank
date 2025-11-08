## 🚀 ASP.NET Core’a Genel Bakış

> 🔤 **Kaynak:** Microsoft Docs — *Overview of ASP.NET Core*
> 🕮 **Çeviri:** Türkçe açıklamalı sürüm
> 💡 **Konu:** Blazor ve ASP.NET Core Giriş

---

### 🌐 ASP.NET Core Nedir?

**ASP.NET Core**, modern web uygulamaları geliştirmek için tasarlanmış,
**çok platformlu (cross-platform)**, **yüksek performanslı** ve **açık kaynaklı (open-source)** bir .NET çatısıdır.

Bu framework:

* Küçük projelerden kurumsal ölçekte dev sistemlere kadar genişleyebilir.
* Windows, macOS ve Linux üzerinde sorunsuz çalışabilir.
* **Blazor**, **Minimal API**, **SignalR** ve **gRPC** gibi modern bileşenleri entegre biçimde sunar.

---

### ⚙️ Temel Özellikler

#### ⚡ Hafif ve Modüler HTTP İşlem Hattı

ASP.NET Core’un HTTP pipeline’ı tamamen modülerdir.
Yani sadece ihtiyacın olan middleware bileşenlerini eklersin, bu da performansı artırır.

#### 🧱 Kestrel Web Server

ASP.NET Core’un varsayılan sunucusudur.

* Platformdan bağımsız çalışır.
* Çok hızlıdır ve ters proxy (reverse proxy) ile Nginx veya IIS arkasında kolayca kullanılabilir.

#### 🧩 Dependency Injection (Bağımlılık Enjeksiyonu)

Framework içine **yerleşik** gelir.
Ek kütüphane kurmaya gerek kalmadan, sınıflar arası bağımlılıklar kolayca yönetilir.

#### 🧭 Ortam Bazlı Konfigürasyon

`appsettings.Development.json`, `appsettings.Production.json` gibi dosyalarla
her ortam için farklı yapılandırmalar kullanabilirsin.

#### 📊 Gelişmiş Logging ve İzleme (Telemetry)

Uygulama loglarını, izleme (tracing) verilerini ve performans metriklerini
tek noktadan yönetmene olanak tanır.

#### 🧠 Blazor ile C# Tabanlı UI Geliştirme

Artık **JavaScript yazmadan** dinamik web arayüzleri oluşturmak mümkün!
Blazor, C# kodunu doğrudan tarayıcıda (WebAssembly) veya sunucuda (SignalR üzerinden) çalıştırır.

#### 🔗 Frontend Framework Entegrasyonu

Blazor ya da Razor Pages uygulamaları, **Angular**, **React**, **Vue** veya **Bootstrap** ile kolayca entegre edilebilir.

#### 🧾 Minimal API

Karmaşık controller yapısı olmadan, yalnızca birkaç satır kodla REST API oluşturabilirsin:

```csharp
var app = WebApplication.CreateBuilder(args).Build();
app.MapGet("/hello", () => "Hello World!");
app.Run();
```

Bu yaklaşım, mikroservis veya basit API’ler için idealdir. 🚀

#### 📡 SignalR

Gerçek zamanlı (real-time) iletişim kurmanı sağlar.
Örnek: canlı sohbet, bildirimler, dashboard güncellemeleri vb.

#### 🔄 gRPC

Yüksek performanslı **Remote Procedure Call (RPC)** servisi kurmana izin verir.
Büyük ölçekli mikroservis mimarilerinde sıkça tercih edilir.

#### 🔐 Güvenlik (Security)

Kimlik doğrulama (Authentication), yetkilendirme (Authorization) ve veri koruma (Data Protection)
özellikleri framework’e gömülüdür.

#### 🧪 Test Edilebilirlik

Unit test ve integration test yazmak kolaydır.
`xUnit`, `MSTest`, `NUnit` gibi framework’lerle doğal uyum sağlar.

#### 🛠️ Geliştirme Araçları

* **Visual Studio 2022**
* **Visual Studio Code**
* CLI komutları (`dotnet new`, `dotnet run`, `dotnet publish`)
  ile tam üretkenlik sağlanır.

---

### 💎 Neden ASP.NET Core?

| Özellik                                           | Açıklama                                                                       |
| ------------------------------------------------- | ------------------------------------------------------------------------------ |
| 🧩 **Tek Çatı (Unified Framework)**               | Web API, MVC, Razor, Blazor hepsi tek ekosistem içinde.                        |
| ⚡ **Yüksek Verimlilik (Full Stack Productivity)** | Tek dil (C#) ile hem frontend hem backend geliştir.                            |
| 🔐 **Güvenli Tasarım (Secure by Design)**         | Güvenlik framework içine entegre edilmiştir.                                   |
| ☁️ **Bulut Hazır (Cloud Ready)**                  | Azure, AWS veya kendi sunucunda kolay dağıtım.                                 |
| 🚀 **Performans & Ölçeklenebilirlik**             | Endüstri standardı performans, yüksek concurrency.                             |
| 🏢 **Kurumsal Güven (Enterprise Proven)**         | Bing, Xbox, Microsoft 365, Azure gibi dev platformlar ASP.NET Core kullanıyor. |

---

### 🧭 Başlarken

> 👩‍💻 “Artık ASP.NET Core öğrenme yolculuğuna başlamanın zamanı geldi!”

İlk adımda:

```bash
dotnet new webapp -n MyFirstAspNetApp
```

Bu komut ile sıfırdan bir ASP.NET Core web uygulaması oluşturulur.
Ardından Visual Studio veya VS Code ile geliştirip çalıştırabilirsin.

---

İstersen bir sonraki adımda bu genel yapının üzerine **Blazor WebAssembly** veya **Blazor Server** örneğiyle devam edelim mi?
