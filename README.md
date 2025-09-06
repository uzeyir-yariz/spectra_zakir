# Astro & Tailwind CSS Başlangıç Kiti

## Özellikler

Kişisel blogunuz için şık ve zengin özelliklere sahip bir platform olan Astro.js Kişisel Blog Şablonunu keşfedin:

- **Astro.js Destekli**: Dinamik ve verimli JavaScript tabanlı deneyim.
- **Tailwind CSS Entegrasyonu**: Şık ve duyarlı bir tasarım sağlar.
- **RSS Beslemesi Desteği**: Hedef kitlenizi zahmetsizce güncel tutar.
- **Markdown Uyumluluğu**: Kolay biçimlendirme ile içerik oluşturmayı kolaylaştırır.
- **Sözdizimi Vurgulama**: Teknoloji meraklıları için kod parçacıklarının okunabilirliğini artırır.
- **SEO Optimize Edilmiş**: Optimum arama motoru görünürlüğü için site haritası içerir.
- **Vercel Dağıtımı:** önceden yapılandırılmış Vercel dağıtımı ve web analitiği.
- **Tercih ettiğiniz çerçeve:** %100 Astro.js şablonu - JS Çerçevenizi seçin (react önceden yüklenmiş)

Estetik ve işlevselliğin kusursuz birleşimini keşfedin ve benzersiz sesinizi dünyayla paylaşın.

## Vitrin

![vitrin](/public/showcase.png ‘AstroPress - Teknoloji Blogu Şablonu’)

## Şablon Entegrasyonları

- @astrojs/tailwind - https://docs.astro.build/en/guides/integrations-guide/tailwind/
- @astrojs/react - https://docs.astro.build/en/guides/integrations-guide/react/
- @astrojs/sitemap - https://docs.astro.build/en/guides/integrations-guide/sitemap/
- @astrojs/rss - https://docs.astro.build/en/guides/rss/
- @vercel/analytics - https://vercel.com/docs/analytics/
- rehype-pretty-code - https://rehype-pretty-code.netlify.app/

## Şablon Yapısı

Astro projenizin içinde aşağıdaki klasörleri ve dosyaları göreceksiniz:

```
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro, `src/pages/` dizininde `.astro` veya `.md` dosyalarını arar. Her sayfa, dosya adına göre bir rota olarak gösterilir.

`src/components/` dizininde özel bir şey yoktur, ancak Astro/React/Vue/Svelte/Preact bileşenlerini buraya yerleştirmeyi tercih ediyoruz.

Görüntüler gibi tüm statik varlıklar `public/` dizinine yerleştirilebilir.

## Komutlar

Tüm komutlar, terminalden projenin kök dizininden çalıştırılır:

| Komut                | Eylem                                           |
| :--------------------- | :------------------------------------------ ----- |
| `npm install`          | Bağımlılıkları yükler                            |
| `npm run dev`          | `localhost:3000` adresinde yerel geliştirme sunucusunu başlatır      |
| `npm run build`        | Üretim sitenizi `./dist/` adresine derler          |
| `npm run preview`      | Dağıtmadan önce derlemenizi yerel olarak önizler     |
| `npm run astro ...`    | `astro add`, `astro check` gibi CLI komutlarını çalıştır |
| `npm run astro --help` | Astro CLI'yi kullanarak yardım al |

## Daha fazla bilgi edinmek ister misiniz?

Astro'nun [belgelerini](https://docs.astro.build) inceleyebilirsiniz.