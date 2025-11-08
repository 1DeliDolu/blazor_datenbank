## 🧩 ASP.NET Core ile Başlarken

---

### 🌐 Giriş

Bu eğitimde, **.NET CLI** (komut satırı aracı) kullanarak bir **ASP.NET Core Blazor Web App** oluşturmayı, çalıştırmayı ve değiştirmeyi öğreneceksin.

**Blazor**, hem **sunucu tarafı render** (server-side rendering) hem de **istemci etkileşimi** (client interactivity) destekleyen modern bir .NET frontend framework’tür.
Yani HTML + C# birleşimiyle JavaScript’e gerek kalmadan dinamik web arayüzleri oluşturabilirsin. 🚀

---

### 🎯 Bu eğitimde öğreneceklerin

* Blazor Web App oluşturmak
* Uygulamayı çalıştırmak
* Kod üzerinde değişiklik yapmak
* Uygulamayı kapatmak

---

## ⚙️ Gereksinimler

1. En güncel **.NET SDK**’yı indir ve kur:
   🔗 [Download .NET](https://dotnet.microsoft.com/download)
2. Komut satırı aracı olarak **CMD**, **PowerShell** veya **VS Code terminali** kullanabilirsin.

---

## 🧱 1. Blazor Web App Oluşturma

Komut satırında, uygun bir klasöre gidip şu komutu çalıştır:

```bash
dotnet new blazor -o BlazorSample
```

> 🔹 `-o` parametresi, proje için **BlazorSample** adlı bir klasör oluşturur.
> 🔹 Bu klasör aynı zamanda proje adını da belirler.

---

## ▶️ 2. Uygulamayı Çalıştırma

Önce oluşturduğun dizine geç:

```bash
cd BlazorSample
```

Ardından uygulamayı izleme modunda başlat:

```bash
dotnet watch
```

Bu komut:

* Uygulamayı derler ve çalıştırır,
* Varsayılan tarayıcını açar,
* Kodda değişiklik yaptığında **otomatik olarak yeniden yükler** 🔁

Blazor Web App, tarayıcıda bir **ana sayfa (Home)** ile açılır.
Sol menüde “**Counter**” sayfasına tıklayarak sayaç bileşenine ulaşabilirsin.

---

## 🧮 3. Uygulamayı Değiştirme

Tarayıcıyı açık bırak.
Blazor’un canlı yeniden yükleme (hot reload) özelliği sayesinde kodu değiştirdiğinde sayfa otomatik güncellenir.

🧭 **Dosya yolu:**

```
Components/Pages/Counter.razor
```

Bu dosyayı açtığında şu kodu göreceksin:

```razor
@page "/counter"

<PageTitle>Counter</PageTitle>

<h1>Counter</h1>

<p role="status">Current count: @currentCount</p>

<button class="btn btn-primary" @onclick="IncrementCount">Click me</button>

@code {
    private int currentCount = 0;

    private void IncrementCount()
    {
        currentCount++;
    }
}
```

### 📘 Kodun açıklaması:

| Satır                                               | Açıklama                                                 |
| --------------------------------------------------- | -------------------------------------------------------- |
| `@page "/counter"`                                  | Bu bileşenin `/counter` URL’sinde çalışacağını belirtir. |
| `<PageTitle>Counter</PageTitle>`                    | Tarayıcı sekmesinde görünen sayfa başlığıdır.            |
| `<p role="status">Current count: @currentCount</p>` | Sayaç değerini ekranda gösterir.                         |
| `<button ... @onclick="IncrementCount">`            | Butona tıklanınca C# metodu (`IncrementCount`) çalışır.  |
| `currentCount++`                                    | Her tıklamada sayaç 1 artar.                             |

---

### 🧠 Kod Değişikliği: Artışı 10’a Çıkaralım

Şu satırı değiştir:

```diff
- currentCount++;
+ currentCount += 10;
```

Dosyayı kaydettiğinde, `dotnet watch` aktif olduğu için tarayıcıda sayfa **otomatik yenilenir.**
Artık butona tıkladığında sayaç **10’ar 10’ar artacaktır**. 🎉

---

## 🧰 4. Uygulamayı Durdurma

1. Tarayıcı sekmesini kapat.
2. Komut satırına dönüp **Ctrl + C** tuşlarına bas.
3. Uygulama kapanacaktır.

---

## 🏁 Tebrikler!

🎉 Artık ilk **Blazor Web App** uygulamanı başarıyla oluşturdun, çalıştırdın, değiştirdin ve kapattın.

---

### 🔗 Sonraki Adımlar

* **Blazor component lifecycle** hakkında bilgi edin.
* **Veri bağlama (Data Binding)** ve **event handling** konularını incele.
* **Entity Framework Core** ile veritabanı bağlantısı kurarak dinamik verilerle çalışmayı öğren.

---
