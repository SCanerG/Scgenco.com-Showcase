# CI/CD — Private Application Automation

[English](../README.en.md) · [Türkçe](../README.tr.md)

The private application repository uses GitHub Actions for continuous integration. Pushes and pull requests trigger lint, TypeScript checks, a production build, unit/SEO tests and selected Chrome browser regressions covering the connected studios, trust pages and customer journeys. Dependencies use a committed lockfile, and actions are pinned to specific commits.

Verified on 15 October 2026: the actual GitHub-hosted Linux run passed lint, type checking, production build, 79 unit tests, 130 SEO checks and 118 browser tests. The delivery stage was skipped because Cloudflare credentials are not yet configured; a passing CI run is not a completed deployment.

The delivery stage is configured to publish the exact tested static artifact to Cloudflare Pages only after successful quality checks. Cloudflare account credentials and the actual Pages project must be configured before activation. **CI is enabled; Cloudflare delivery is configured but not activated or verified yet.** This is not a claim of an already deployed live website.

Source code, workflow files, credentials, build artifacts and diagnostic reports remain in the private development environment. This public repository contains presentation documents and reviewed screenshots only. It is not used to build or deploy the application.

## Türkçe

Private uygulama deposunda GitHub Actions ile sürekli entegrasyon kullanılır. Push ve pull request işlemlerinde lint, TypeScript, üretim derlemesi, birim/SEO testleri ve seçilmiş Chrome tarayıcı regresyonları otomatik çalışır. Stüdyolar, bilgilendirme sayfaları ve müşteri yolculukları bu kapsamda doğrulanır.

15 Ekim 2026 tarihinde gerçek GitHub Linux çalışmasında lint, TypeScript, üretim derlemesi, 79 birim testi, 130 SEO kontrolü ve 118 tarayıcı testi başarılı oldu. Cloudflare erişimi henüz yapılandırılmadığı için dağıtım aşaması atlandı; başarılı CI, tamamlanmış dağıtım anlamına gelmez.

Dağıtım aşaması, başarılı testlerden geçen aynı statik çıktıyı Cloudflare Pages'e aktaracak şekilde hazırlanmıştır. **CI etkindir; Cloudflare dağıtımı yapılandırılmıştır ancak erişim/proje ayarları tamamlanmadan etkin veya doğrulanmış değildir.** Canlı sitenin yayımlandığı iddia edilmez.

Kaynak kod, workflow dosyaları, sırlar, derleme çıktıları ve hata raporları private alanda kalır. Public showcase yalnızca sunum belgeleri ve incelenmiş ekran görüntülerini içerir; uygulamanın derleme/dağıtım kaynağı değildir.
