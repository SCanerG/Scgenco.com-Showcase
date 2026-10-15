# CI/CD — Private Application Automation

[English](../README.en.md) · [Türkçe](../README.tr.md)

The private application repository uses GitHub Actions for continuous integration. Pushes and pull requests trigger lint, TypeScript checks, a production build, unit/SEO tests and selected Chrome browser regressions covering the connected studios, trust pages and customer journeys. Dependencies use a committed lockfile, and actions are pinned to specific commits.

The delivery stage is configured to publish the exact tested static artifact to Cloudflare Pages only after successful quality checks. Cloudflare account credentials and the actual Pages project must be configured before activation. **CI is enabled; Cloudflare delivery is configured but not activated or verified yet.** This is not a claim of an already deployed live website.

Source code, workflow files, credentials, build artifacts and diagnostic reports remain in the private development environment. This public repository contains presentation documents and reviewed screenshots only. It is not used to build or deploy the application.

## Türkçe

Private uygulama deposunda GitHub Actions ile sürekli entegrasyon kullanılır. Push ve pull request işlemlerinde lint, TypeScript, üretim derlemesi, birim/SEO testleri ve seçilmiş Chrome tarayıcı regresyonları otomatik çalışır. Stüdyolar, bilgilendirme sayfaları ve müşteri yolculukları bu kapsamda doğrulanır.

Dağıtım aşaması, başarılı testlerden geçen aynı statik çıktıyı Cloudflare Pages'e aktaracak şekilde hazırlanmıştır. **CI etkindir; Cloudflare dağıtımı yapılandırılmıştır ancak erişim/proje ayarları tamamlanmadan etkin veya doğrulanmış değildir.** Canlı sitenin yayımlandığı iddia edilmez.

Kaynak kod, workflow dosyaları, sırlar, derleme çıktıları ve hata raporları private alanda kalır. Public showcase yalnızca sunum belgeleri ve incelenmiş ekran görüntülerini içerir; uygulamanın derleme/dağıtım kaynağı değildir.
