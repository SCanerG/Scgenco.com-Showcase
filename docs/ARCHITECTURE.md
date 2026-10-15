# Architecture Overview / Genel Mimari

[English](../README.en.md) · [Türkçe](../README.tr.md)

The current platform combines static content delivery with browser-based interactive concepts. No backend, database or authentication is implemented. Detailed proprietary implementation and infrastructure settings are excluded from this public document.

Mevcut platform statik içerik sunumunu tarayıcıdaki etkileşimli konseptlerle birleştirir. Backend, veritabanı ve kimlik doğrulama uygulanmamıştır. Özel uygulama ayrıntıları ve altyapı ayarları bu açık belgeye dahil edilmez.

## System / Sistem

```mermaid
flowchart LR
  Site["Static portfolio and service content"] --> Visitor["Visitor browser"]
  Visitor --> Studios["Interactive concept studios"]
  Visitor --> Music["Shared audio experience"]
  Studios --> Brief["Project brief"]
  Brief --> Handoff["Visitor-controlled email draft or file"]
```

## Experience components / Deneyim bileşenleri

```mermaid
flowchart TD
  Shell["Bilingual navigation and theme"] --> Pages["Portfolio, services and articles"]
  Shell --> Web["Website Studio"]
  Shell --> Booking["Appointment Studio demo"]
  Shell --> Song["Music Studio"]
  Shell --> Estate["Real Estate Studio demo"]
  Web --> Brief["Unified project brief"]
  Booking --> Brief
  Song --> Brief
  Estate --> Brief
```

## User data flow / Kullanıcı veri akışı

Real Estate Studio shares one fictional portfolio across website, mobile and agency dashboard previews. It supports local customization, validated concept files and a project brief. The illustrative map, leads and viewings do not connect to live providers or customer systems.

Emlak Stüdyosu web, mobil ve ofis panelinde aynı kurgusal portföyü kullanır. Yerel özelleştirme, doğrulanan konsept dosyaları ve proje özeti desteklenir. Temsili harita, adaylar ve gezdirmeler canlı sağlayıcı veya müşteri sistemine bağlanmaz.

```mermaid
flowchart LR
  Idea["Describe an idea"] --> Concept["Customize and preview"]
  Concept --> Review["Review a validated concept"]
  Review --> Brief["Attach to project brief"]
  Brief --> Export["Explicit local export or email preparation"]
```

## Delivery / Sunum ve dağıtım

```mermaid
flowchart LR
  Private["Private application development"] --> Build["Static production build"]
  Build --> Hosting["Static hosting - not deployed yet"]
  Hosting --> Browser["Visitor experience"]
  Showcase["Public documentation showcase"] --> Reader["GitHub visitors"]
```

Custom text stays original when interface language changes. Local saves and file exports require explicit visitor actions. Demo booking records are fictional; email drafts are not sent automatically. A future authenticated owner platform is separately [planned](ROADMAP.md), not part of the current diagrams.

Arayüz dili değişince özel metinler özgün kalır. Yerel kayıt ve dışa aktarım açık eyleme bağlıdır. Demo randevular kurgusaldır; e-posta taslakları otomatik gönderilmez. Kimliği doğrulanan sahip platformu ayrıca [planlanmaktadır](ROADMAP.md); mevcut diyagramların parçası değildir.
