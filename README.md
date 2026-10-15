# Resmen · Claude Code eklentisi

Türk mevzuatına yalnızca resmî kaynaklardan, madde düzeyinde erişim. Sorunuzu günlük dille sorarsınız; cevap
kanun, yönetmelik, tebliğ, özelge ve kararların ilgili maddesi, kaynak adresi ve son kontrol tarihiyle gelir.

Pilot şu an **davetlidir**. Davet kodunuz yoksa kurulum yapılır ama giriş açılmaz.

## Kurulum

Aşağıdaki satırı Claude Code'a yapıştırıp Enter'a basın. Başındaki `!` işareti satırı komut olarak çalıştırır
(terminalde çalıştırmak isterseniz `!` olmadan yapıştırın):

```
! claude plugin marketplace add OzayArtunBoran/resmen --scope user && claude plugin install hukuk@resmen --scope user && claude mcp add --transport http --scope user hukuk https://mcp.resmen.com.tr/mcp
```

Sonra Claude Code'u kapatıp yeniden açın, `/mcp` yazın, `hukuk`'u seçin ve tarayıcıda açılan sayfaya davet kodunuzu
girin.

## Eklentide ne var

- **`hukuk` becerisi:** Hukuki sorularda cevap disiplini: önce resmî kaynaktan madde, sonra cevap; her iddiada madde,
  alıntı, adres ve son kontrol tarihi. Beceri etkinken WebSearch ve WebFetch araçları kapalıdır.
- **`hukuk-arastirmaci` ajanı:** Bir olayın bütün hukuki boyutlarını (vergi, KVKK, tüketici, iş/SGK, ticari ileti,
  sözleşme …) tek tek kontrol eder; ilgisiz bulduğunu gerekçesiyle yazar. Ajanın tek aracı Resmen'dir: internet
  araması, web sayfası, dosya ya da terminal erişimi yoktur.

Eklenti bir MCP sunucusu taşımaz. Bağlantıyı üçüncü komut (`claude mcp add`) kurar.

## Ne yapmaz

- İnternette arama yapmaz; haber, blog, forum ya da özel hukuk sitelerine bakmaz.
- Hukuki görüş vermez, avukat ya da mali müşavirin yerini almaz. Uzmana hangi soruyla gidileceğini netleştirir.

Resmen bir kamu kurumu değildir.
