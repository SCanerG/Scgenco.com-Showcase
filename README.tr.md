# Scgenco.com — Kişisel Portfolyo ve Dijital Hizmetler Platformu

[Dil seçimi](README.md) · [English](README.en.md)

![Next.js](https://img.shields.io/badge/Next.js-16.4-black) ![React](https://img.shields.io/badge/React-19.3-149eca) ![TypeScript](https://img.shields.io/badge/TypeScript-5.9-3178c6) ![Status](https://img.shields.io/badge/Source-private-6d5ce7)

## Genel bakış

Scgenco.com, Sabri Caner Genco’nun profesyonel portfolyo ve dijital hizmetler sitesidir. Mühendislik çalışmalarının açık sunumunu, geliştirme veya yaratıcı üretim başlamadan müşterinin ihtiyacını anlatmasını sağlayan etkileşimli araçlarla birleştirir. Potansiyel müşteriler, iş ortakları, işe alım uzmanları ve teknik inceleyenler için tasarlanmıştır.

## Temel özellikler

- İçerik, stüdyo şablonları, randevu demoları ve proje özetlerinde Türkçe/İngilizce deneyim.
- Altı kategoride on iki çok sayfalı konsept, canlı düzenleme, yerel görseller ve duyarlı önizlemeler sunan Web Sitesi Stüdyosu.
- Dört kurgusal sektör, hizmet/ekip düzenleme, simülasyon uygunluk, randevu ve yönetim ekranları sunan Randevu Sistemi Stüdyosu.
- On iki kişisel/ticari kategori, müzik tercihleri, özgün hikâye/sözler ve anlaşılır şarkı taslağı sunan Müzik Stüdyosu.
- Altı işletme profili ve altı şablonla 18 kurgusal ilanı web, mobil ve ofis panelinde deneyimleten Emlak Stüdyosu; filtre, galeri, favori, karşılaştırma ve temsili harita.
- Yeni SG marka kimliği, iki dilli SSS ve gizlilik/hizmet bilgilendirme sayfaları.
- İsteğe bağlı stüdyo tasarımını taşıyan ve e-posta taslağı/indirilebilir dosya hazırlayan ortak proje özeti.
- Sahibinin sağladığı Türkçe/İngilizce özgün kayıtlar; desteklenen iç gezinmede kesintisiz ses deneyimi.
- Açık/koyu tema, duyarlı düzen, erişilebilir etiketler ve klavye etkileşimi.
- Hizmet kataloğu, mühendislik proje incelemeleri, Markdown yazılar ve doğrudan iletişim.

## Teknoloji yığını

Next.js 16.4, React 19.3 ve TypeScript 5.9; Tailwind CSS 4.3/PostCSS ve özel CSS; Motion, Lucide, react-markdown ve yerel Geist. React Context/hook tarayıcı durumunu yönetir. Node/npm/Turbopack statik varlık üretir; TypeScript, ESLint, Node testleri, Playwright ve axe-core doğrulama sağlar. [Doğrulanan yığın](docs/TECH_STACK.md).

## Mimari özeti

Site statik HTML, CSS, JavaScript ve medya olarak önceden üretilir. Stüdyolar ve proje özeti tarayıcıda çalışır. Ziyaretçi yerel taslak kaydını veya dışa aktarımı açıkça seçer. Ortak ses deneyimi sayfa yüzeylerini bağlar. [Mimari diyagramlar](docs/ARCHITECTURE.md).

Şu anda üretim backend’i, veritabanı, kimlik doğrulama veya gerçek sahip yönetim sistemi yoktur. Randevu paneli kurgusal demodur. E-posta hazırlama otomatik gönderim yapmaz; müzik stüdyosu ses üretmez; alışveriş önizlemesi ödeme işlemez.

Emlak ofis panelindeki ilan, aday ve gezdirme etkileşimleri de kurgusal tarayıcı simülasyonudur. Harita yerel ve şematiktir; canlı harita veya gerçek rezervasyon değildir. Mobil önizleme, yayımlanmış bir Android/iOS uygulaması değildir. Bilgilendirme sayfaları hukuki incelemenin tamamlandığı iddiasını taşımaz.

## Teknik öne çıkanlar

Kararlı yapılandırma kimlikleri çevrilmiş etiketlerden ayrıdır. Örnek içerik seçilen dile uyar; özel metinler özgün kalır. Sürümlü dosyalar mevcut çalışmayı değiştirmeden önce doğrulanır. Ortak tasarım ekleri farklı stüdyoları tek talep akışına bağlar. Önizleme stilleri çevredeki açık/koyu temadan bağımsızdır. Tembel editör yüklemesi başlangıç deneyimini odaklı tutar.

## Ekran görüntüleri

Gerçek uygulamadan, yerleşik kurgusal örneklerle alınmıştır. Müşteri kaydı, kimlik bilgisi, özel altyapı veya üretim yönetim ekranı gösterilmez.

![Türkçe web şablon galerisi](assets/screenshots/website-tr.webp)
![Türkçe kurgusal randevu konsepti](assets/screenshots/appointment-tr.webp)
![Türkçe müzik stüdyosu tanıtımı](assets/screenshots/music-tr.webp)
![Türkçe Emlak Stüdyosu — kurgusal örnek ilanlar](assets/screenshots/real-estate-tr.webp)

[Görsel notları](assets/screenshots/README.md).

## Geliştirme yol haritası

Private uygulama deposunda otomatik kalite kontrolleri için GitHub Actions CI kullanılır. Cloudflare Pages dağıtımı başarılı kontrollerin arkasında tanımlıdır; hesap/proje ayarlarını bekler ve henüz etkin veya doğrulanmış değildir. [CI/CD süreci ve durumu](docs/CI_CD.md).

Planlananlar: güvenli sahip paneli, talep/müşteri yönetimi, hizmet takibi, teklif hazırlama ve onay, sipariş durumu, otomatik işlem e-postaları/teslimat takibi, iletişim geçmişi ve panel analitiği. Bunlar tamamlanmış özellikler değildir. [Yol haritası ve durum](docs/ROADMAP.md).

## Canlı site

Henüz dağıtılmış veya doğrulanmış değil. Scgenco.com proje/planlanan alan adı kimliğidir; yalnızca gerçek dağıtım doğrulandıktan sonra canlı bağlantı eklenecektir. Cloudflare Pages hazırlığı özel belgelerde yer alır; bu yayın görevinde hosting dağıtımı yapılmadı.

## İletişim ve kaynak mahremiyeti

[Sabri Caner Genco’ya e-posta](mailto:s.canergenco@gmail.com) · [LinkedIn](https://www.linkedin.com/in/sabri-caner-genco-762776216/) · [GitHub](https://github.com/SCanerG)

Bu showcase yalnızca dokümantasyondur. Özel uygulama kaynağı, yapılandırma, yaratıcı taslaklar ve müşteri verisi dışlanır. Telif ve marka/medya hakları sahiplerinde kalır; bu depo kaynak kod lisansı vermez.
