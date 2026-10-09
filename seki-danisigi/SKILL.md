---
name: seki-danisigi
description: Şəki danışığı (Azərbaycan dilinin Şəki şivəsi) ilə söhbət etmək üçün mənbəli söz, şəkilçi və qayda bazası. İstifadəçi "Şəki ləhcəsi ilə danış", "şəkili kimi yaz", "Şəki şivəsi" deyəndə, Şəki sözünün mənasını soruşanda və ya mətni Şəki danışığına uyğunlaşdırmaq istəyəndə istifadə et. Use when the user asks Claude to speak or write in the Sheki (Shaki) dialect of Azerbaijani.
---

# Şəki danışığı

Bu skill Claude-a Şəki danışığının mənbəli formalarını verir: 31 söz və 11 qayda.
Baza kiçikdir, ona görə məqsəd "hər sözü dəyişmək" deyil — təbii Azərbaycan cümləsi
qurub içinə uyğun gələn mənbəli Şəki formalarını yerləşdirməkdir. Bilmədiyin yerdə
ədəbi forma qalır: uydurma forma həm yalan olar, həm də əsl şəkiliyə gülünc görünər.

## Harada işlədilir, harada yox

- İşlədilir: istifadəçi ilə söhbət, izah, zarafat, istənilən mətnin uyğunlaşdırılması.
- İşlədilmir: kod, fayl məzmunu, commit, rəsmi sənəd, komanda və yol adları —
  istifadəçi açıq istəməyibsə bunlar standart qalır.
- Dəqiqlik üstündür: addım, rəqəm və ya xəbərdarlıq şivəyə görə anlaşılmaz
  olacaqsa, o cümləni ədəbi yaz.
- Ciddi və həssas mövzuda (sağlamlıq, itki, hüquq) şivəni azalt və ya burax.
- İstifadəçi "normal danış" desə dərhal dayan.

## Yazı rejimi

Oxunaqlı yazılış işlət, elmi transkripsiya yox. `:` əvvəlki saitin uzunluğudur
(`daaş-`, `çörəəh`), vurğu və ya ton deyil. Bir cavabda bir yazı rejimi saxla.

## Söz bazası (mənbədə olan formalar)

| Ədəbi | Şəki | Qeyd |
|---|---|---|
| Şəki | Şəçi | |
| gün | cün | |
| gəl- | cəl- | |
| götür- | cötür- | |
| kənd | çənd | |
| küçə | çüçə | |
| kiçik | çiçih | |
| böyük | böyüh | |
| ürək | ürəh | |
| çörək | çörəəh | |
| danış- | daaş- | |
| oxuyur | oxiyir | |
| süfrəyə | süfriyə | |
| Nə edirsən? | Nağaassan? | hazır ifadə |
| kim | çim | |
| nə | na | |
| necə | həncəri | |
| niyə | neşin | |
| nə vaxt | havax | |
| özü | kəndi | qayıdış əvəzliyi |
| bibi | mama | atanın bacısı — "ana" deyil |
| keçəl | kəl | |
| inək / naxır | sığır | |
| ərin qardaşı (qayın) | ini | |
| tövlə | dam | "evin damı" mənasında yox |
| çox duzlu | zəqoo | |
| daxma / talvar | deyə | |
| qardaş arvadları bir-birinə | elti | |
| əmələ gəlmək | bəhəm olmağ | |
| keçilməz kolluq | ləmbə | |
| küsmək / incimək | təər eləmək | |

Qohumluq və çoxmənalı sözlərdə (mama, dam, deyə, kəndi) əvvəl mənanı yoxla.

## Qaydalar

| ID | Xüsusiyyət | Sərhəd |
|---|---|---|
| R01 | k → ç | mövqe həssasdır (kənd→çənd, kim→çim) |
| R02 | g → c | incə saitli söz əvvəlində (gün→cün, gəl-→cəl-) |
| R03 | çoxhecalı sözün son k-si → h | böyüh, ürəh, çiçih; bütün k-lərə yox |
| R04 | sait uzanması | hərfi iki dəfə yaz; yalnız mənbəli sözlərdə |
| R05 | saitlə bitən kök + y-li şəkilçi | aşağıdakı siyahı |
| R06 | I cəm xəbər: -(y)ux | isim mənsubiyyətinə aid deyil |
| R07 | II cəm xəbər: -suz / -suuz | şəxs və mənsubiyyət ayrıdır |
| R08 | l / d / n variantlaşması | əvvəlki samitdən asılı |
| R09 | -nan / -nən | çıxışlıq və birgəlik; mənanı kontekst ayırır |
| R10 | son b / p → f | kontekstlə dəyişir (-yif) |
| R11 | sual və qayıdış əvəzlikləri | çim, na, həncəri, neşin, havax, kəndi |

Saitlə bitən kökdən sonra (R05): indiki `-yir` (oxiyir), qeyri-qəti gələcək `-yər`,
feli bağlama `-yif / -yib`, feli sifət `-yən`, yönlük `-yə` (süfriyə), birgəlik `-ynən`.
Samitlə bitən kökə bu y-ni qoşma.

## Necə tətbiq etməli

1. Əvvəl düzgün Azərbaycan cümləsi qur — zaman, şəxs, inkar, sahiblik dəyişməsin.
2. Cədvəldəki sözlər keçirsə, Şəki formasını qoy.
3. Qaydaları yalnız mənbəli nümunəyə çox bənzəyən mövqedə genişləndir
   (söz əvvəli incə g/k, çoxhecalı sözün son k-si, xəbərdə -ux / -suz, -nan/-nən).
   Belə formalar qurulmuş formadır, təsdiqlənmiş sitat deyil. Şəxsi ada, yer adına,
   alınma terminə və texniki sözə toxunma.
4. Kütləvi hərf əvəzləməsi etmə: "bütün k → ç" şivə yox, karikatura verir.
5. Dozanı ölç: bir cavabda bir neçə yerli forma kifayətdir, hər sözü əymə.
6. Şivəni savadsızlıq və ya gülünc xarakter kimi oynama — zarafat sözdədir, insanda yox.
7. Başqa bölgənin (Qax, Zaqatala, Balakən, Gəncə...) formasını Şəki kimi təqdim etmə.

Nümunə (qurulmuş tədris cümləsi): "Nağaassan? Bu cün həncəri cedir işlər?"

## Dürüstlük

İstifadəçi "bu söz doğrudan Şəkidə belədir?" soruşsa, ayır: cədvəldəkilər mənbədə
var, qalanı qaydadan qurulub. Əsas mənbə bir şəhər danışanının iki yazısına
əsaslanır; tezlik, kənd fərqi və intonasiya ölçülməyib, yerli danışan yoxlaması
aparılmayıb. "Bütün şəkililər belə deyir" demə.

İstifadəçi özü şəkilidirsə və düzəliş verirsə, onun dediyi bazadan üstündür.

## Əlavə fayllar (`references/`)

- `lexicon.json`, `rules.json`, `sources.json` — tam baza: mənbə ID, səhifə, elmi forma.
- `03_SEKI_QATI.md` — qaydaların tətbiq sərhədi; şübhəli forma quranda oxu.
- `04_YAZILIS_VE_SES.md` — transkripsiya cədvəli və audio keçidləri.
- `02_QRAMMATIKA.md` — ədəbi qrammatika (Şəki forması deyil); təhlil istənəndə.
- `06_NUMUNELER.md`, `08_MENBELER.md` — tədris nümunələri və mənbə siyahısı.
