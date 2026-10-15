# CI/CD — Private Application Automation

[English](../README.en.md) · [Türkçe](../README.tr.md)

The private application repository uses GitHub Actions for continuous integration. Pushes and pull requests trigger lint, TypeScript checks, a production build, unit/SEO tests and selected Chrome browser regressions covering the connected studios, trust pages and customer journeys. Dependencies use a committed lockfile, and actions are pinned to specific commits.

Verified on 15 October 2026: GitHub-hosted Linux checks passed lint, type checking, production build, 79 unit tests, 130 localized SEO routes plus the root entry, 131 exported HTML pages and 119 browser tests. The Cloudflare Pages delivery stage also completed successfully using the tested artifact.

The delivery stage publishes the exact tested static artifact to Cloudflare Pages only after successful quality checks. **CI and automatic Pages delivery are enabled, and the first pipeline deployment succeeded.** The production custom domain's DNS/TLS and live indexing remain unverified; successful artifact publication does not establish that the intended domain serves the application.

Source code, workflow files, credentials, build artifacts and diagnostic reports remain in the private development environment. This public repository contains presentation documents and reviewed screenshots only. It is not used to build or deploy the application.

## Türkçe

Private uygulama deposunda GitHub Actions ile sürekli entegrasyon kullanılır. Push ve pull request işlemlerinde lint, TypeScript, üretim derlemesi, birim/SEO testleri ve seçilmiş Chrome tarayıcı regresyonları otomatik çalışır. Stüdyolar, bilgilendirme sayfaları ve müşteri yolculukları bu kapsamda doğrulanır.

15 Ekim 2026 tarihinde gerçek GitHub Linux çalışmasında lint, TypeScript, üretim derlemesi, 79 birim testi, kök giriş ve 130 yerelleştirilmiş rota için SEO denetimi, 131 HTML çıktısı ve 119 tarayıcı testi başarılı oldu. Cloudflare Pages dağıtım aşaması da test edilen çıktıyla başarıyla tamamlandı.

Dağıtım aşaması, başarılı testlerden geçen aynı statik çıktıyı Cloudflare Pages'e aktarır. **CI ve otomatik Pages yayını etkindir; ilk pipeline dağıtımı başarılıdır.** Üretim özel alan adının DNS/TLS bağlantısı ve canlı indeksleme durumu henüz doğrulanmış değildir; dosya yüklemesinin başarısı alan adı bağlantısının tamamlandığı anlamına gelmez.

Kaynak kod, workflow dosyaları, sırlar, derleme çıktıları ve hata raporları private alanda kalır. Public showcase yalnızca sunum belgeleri ve incelenmiş ekran görüntülerini içerir; uygulamanın derleme/dağıtım kaynağı değildir.
