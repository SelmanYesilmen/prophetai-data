# prophetai-data

ProphetAI Real Estate (Emlak) uygulamasının çalışma zamanında indirdiği **kamuya
açık istatistik dosyaları**. Uygulama kodu bu depoda değildir.

| Dosya | İçerik | Kaynak | Yenileme |
|---|---|---|---|
| `kfe.json` | TCMB Konut Fiyat Endeksi — Türkiye + 19 İBBS bölgesi, aylık, 2015-01'den itibaren (baz 2023=100) | [TCMB EVDS](https://evds3.tcmb.gov.tr) | ayda bir, TCMB yayınından sonra (`npm run publish:kfe`) |

Dosya üretilmiştir; elle düzenlenmez. Şema ve doğrulama kuralları uygulama
tarafında (`services/kfeRemoteRules.ts`) tanımlıdır — biçime uymayan dosya
cihazda reddedilir, uygulama kendi gömülü kopyasıyla çalışmaya devam eder.

Uygulama bu dosyayı indirirken hiçbir kullanıcı verisi göndermez.
