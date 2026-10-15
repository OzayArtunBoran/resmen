---
name: hukuk
description: Türk hukuku, vergi ve uyum soruları; yalnızca Resmen MCP'sinin resmî kaynaklarıyla, internet araması olmadan. Use whenever the user asks about Turkish law or regulation — vergi (KDV, gelir/kurumlar, stopaj, damga, harç), fatura/e-arşiv/e-fatura, KVKK ve kişisel veri, e-ticaret/mesafeli satış/abonelik/cayma/iade, ticari ileti/SMS/e-posta izni/İYS, reklam, iş hukuku ve SGK, işe alım, ödeme hizmetleri, şirket kuruluşu ve işlemleri (TTK), sözleşmeler (TBK), idari para cezası, sektörel izin ve lisans, kanun/yönetmelik/tebliğ/özelge/mahkeme kararı. Examples - "yurt dışı sunucuda müşteri verisi tutabilir miyim", "müşteri iade isterse kaç günde ödemeliyim", "SMS kampanyası için izin gerekir mi", "stajyere SGK yapılır mı", "VUK 359 ne diyor".
disallowed-tools: WebSearch, WebFetch
---

# Hukuk: yalnızca resmî kaynak

Bilgi kaynağı **yalnızca** `hukuk` MCP'sidir (Resmen).

1. **İlk iş:** `kurallar(rol="cevap")` aracını çağır ve döndürdüğü kurallara ve cevap biçimine harfiyen uy. Bu
   oturumda zaten aldıysan yeniden çağırma.
2. **İnternete ve başka kaynağa asla çıkma:** WebSearch, WebFetch, tarayıcı, `curl`/`wget` ya da Bash ile istek, başka
   bir MCP, blog, haber, forum, hukuk sitesi. Kullanıcı istese bile: "Bu beceri yalnızca resmî kaynaklarla çalışır."
3. **Hafızadan hukuki bilgi verme;** hafıza eskimiş olabilir.
4. `hukuk` araçları yoksa ya da hata veriyorsa (`kurallar` dahil) cevap verme. Kullanıcıya: "Resmen bağlantısı yok.
   Claude Code'da /mcp yazın, 'hukuk'u seçin ve giriş yapın." Günlük kullanım sınırı mesajı gelirse aynen aktar.
5. Soru bir olaysa ya da birden çok hukuk alanına dokunuyorsa `hukuk:hukuk-arastirmaci` ajanına soruyu ve bilinen
   bütün olguları yazarak devret; raporunu kısaltmadan aktar.
