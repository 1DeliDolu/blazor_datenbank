
## 🌐 ASP.NET Core Web UI Seçenekleri

> 💡 ASP.NET Core, web arayüzü (UI) geliştirmek için çeşitli yaklaşımlar sunan tam kapsamlı bir çerçevedir.
>
> Yeni projeler için **Blazor** önerilir.

---

### ⚡ 1. Blazor

Blazor, **C#** ile hem istemci (WebAssembly) hem de sunucu (Server) tarafında çalışan, modern bir web UI framework’tür.

#### 🚀 Avantajları

* 🔁 **Yeniden kullanılabilir bileşen modeli**
* ⚡ **Verimli diff tabanlı render sistemi**
* 🌍 **WebAssembly veya Server modeliyle esnek çalışma**
* 💬 **JavaScript ile etkileşim (Interop)**
* 🧩 **Sunucu veya istemci tarafında render seçeneği**
* 🧠 **İstemci ve sunucu arasında ortak C# kod paylaşımı**
* ⚙️ **Statik render + progressive enhancement desteği**

#### 📘 Başlangıç Rehberi:

[Build your first Blazor app](https://learn.microsoft.com/aspnet/core/blazor)

---

### 📄 2. Razor Pages

 **Razor Pages** , MVC’nin sadeleştirilmiş bir versiyonudur.

Her sayfa kendi kod-behind dosyasına sahiptir ve **sunucu tarafında render edilir.**

#### 🚀 Avantajları

* 🧠 UI kodu ve mantık birbirinden ayrıdır ama aynı klasörde tutulur.
* 🧩 Basit dosya ve klasör düzeni.
* ✅ Test edilebilir ve büyük uygulamalara ölçeklenebilir.

#### 📘 Başlangıç Rehberi:

[Tutorial: Get started with Razor Pages in ASP.NET Core](https://learn.microsoft.com/aspnet/core/razor-pages)

---

### 🧭 3. MVC (Model-View-Controller)

 **ASP.NET Core MVC** , klasik ve olgun bir mimaridir.

Uygulama üç katmandan oluşur:

* **Model:** Veri ve iş mantığı
* **View:** Görsel arayüz
* **Controller:** Kullanıcı isteklerini işler, model ile çalışır, uygun view’ı döner.

#### 🚀 Avantajları

* 🔍 **Net ayrılmış sorumluluklar (Separation of Concerns)**
* 🏗️ **Büyük projeler için olgun yapı**
* 🔄 **Esnek ve sürdürülebilir mimari**

#### 📘 Başlangıç Rehberi:

[Get started with ASP.NET Core MVC](https://learn.microsoft.com/aspnet/core/mvc)

---

### 🧠 4. SPA (Single Page Application) — Angular / React / Vue

ASP.NET Core, modern JavaScript framework’leriyle entegre çalışabilir.

Projeni Angular, React veya Vue ile **ön uç (frontend)** olarak kurabilir, **ASP.NET Core’u backend API** olarak kullanabilirsin.

#### 🚀 Avantajları

* 🌐 Tarayıcı zaten JS çalıştırabildiği için hızlıdır.
* 👥 Geniş topluluk ve kütüphane ekosistemi.
* 🔄 Blazor benzeri istemci tarafı etkileşimi.

#### ⚠️ Dezavantajları

* 🧩 Farklı diller ve araçlar (JS + C#)
* ♻️ Kod paylaşımı zor (bazı mantıklar tekrarlanır)

#### 📘 Başlangıç Rehberleri:

* [Create an ASP.NET Core app with Angular](https://learn.microsoft.com/aspnet/core/spa/angular)
* [Create an ASP.NET Core app with React](https://learn.microsoft.com/aspnet/core/spa/react)
* [Create an ASP.NET Core app with Vue](https://learn.microsoft.com/aspnet/core/spa/vue)

---

### 🔗 5. Karma Kullanım — MVC veya Razor Pages + Blazor

ASP.NET Core mimarisi, **Blazor bileşenlerini** MVC veya Razor Pages içinde **entegre etmeye** izin verir.

#### 🚀 Avantajları

* ⚡ **Server-side prerendering** ile daha hızlı yükleme.
* 💬 **Blazor Component Tag Helper** ile etkileşimli bileşen ekleme.
* 🧩 Mevcut MVC veya Razor uygulamalarına modern dinamik bileşenler katma.

#### 📘 Rehber:

[Integrate ASP.NET Core Razor components with MVC or Razor Pages](https://learn.microsoft.com/aspnet/core/blazor/integrate-components)

---

## 🧭 Özet Karşılaştırma

| Model                               | Render Tarafı       | Kod Dili              | Öne Çıkan Özellik                            |
| ----------------------------------- | -------------------- | --------------------- | ------------------------------------------------ |
| **Blazor Server/WebAssembly** | İstemci veya Sunucu | C#                    | Full-stack C# ile web geliştirme                |
| **Razor Pages**               | Sunucu               | C#                    | Basit, sayfa bazlı yapı                        |
| **MVC**                       | Sunucu               | C#                    | Model-View-Controller mimarisi                   |
| **SPA (Angular/React/Vue)**   | İstemci             | JavaScript/TypeScript | Modern JS tabanlı ön yüz                      |
| **MVC + Blazor**              | Sunucu + İstemci    | C#                    | Hibrit yaklaşım (interaktif UI + klasik yapı) |

---
