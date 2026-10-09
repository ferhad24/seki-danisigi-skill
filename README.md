# Şəki danışığı — Claude üçün skill

Claude-a Şəki şivəsi ilə danışmağı öyrədən skill. Yazırsan "Şəki ləhcəsi ilə danış" —
o da cavab verir: **"Nağa:ssan? Bu cün həncəri cedir işlər?"**

*A Claude skill for chatting in the Sheki (Shaki) dialect of Azerbaijani, built on a
small source-backed lexicon instead of made-up forms.*

## İçində nə var

- 31 mənbəli söz və ifadə: `həncəri` (necə), `neşin` (niyə), `havax` (nə vaxt),
  `cün` (gün), `çörə:h` (çörək), `zəqo:` (çox duzlu)...
- 11 səs və şəkilçi qaydası: k → ç, g → c, son k → h, `-yir`, `-ux`, `-suz`, `-nan / -nən`.
- Hər formanın mənbəsi və səhifəsi (`references/lexicon.json`, `rules.json`, `sources.json`).
- Claude üçün davranış qaydası: bilmədiyi yerdə forma uydurmur, ədəbi sözü saxlayır;
  kod və rəsmi sənədə toxunmur; şivəni karikaturaya çevirmir.

## Quraşdırma

**Claude Code:** `seki-danisigi` qovluğunu skill qovluğuna köçür.

```bash
git clone https://github.com/ferhad24/seki-danisigi-skill
cp -r seki-danisigi-skill/seki-danisigi ~/.claude/skills/
```

Windows-da hədəf qovluq: `C:\Users\<ad>\.claude\skills\`

**claude.ai:** `seki-danisigi` qovluğunu ZIP et və Settings → Capabilities → Skills
bölməsindən yüklə.

Sonra sadəcə yaz: *"Mənimlə Şəki ləhcəsi ilə danış."*

## Dəqiqlik sərhədi

Bu, tam Şəki lüğəti deyil — kiçik, amma mənbəli birinci versiyadır.

- Əsas mənbə bir şəhər danışanının iki yazısına əsaslanan məqalədir.
- Yerli danışanla yoxlama aparılmayıb; tezlik, kənd fərqləri və intonasiya ölçülməyib.
- Cədvəldən kənar formaları Claude qaydadan qurur — bunlar təsdiqlənmiş sitat deyil.

Şəkilisənsə və səhv görürsənsə, issue aç və ya düzəliş göndər. Yeni söz əlavə edəndə
harada və kimdən eşitdiyini yaz.

## Mənbələr

Baza "Şəki Dil Paketi v1" (10 oktyabr 2026) əsasında hazırlanıb. Əsas mənbələr:

- *The Sheki dialect of Northern Azeri* — https://dergipark.org.tr/en/pub/tdd/article/1412621
- *Azərbaycan dialektologiyası*
- *Azərbaycan dilinin dialektoloji lüğəti* (azleks.az)

Tam siyahı: [seki-danisigi/references/08_MENBELER.md](seki-danisigi/references/08_MENBELER.md).
Mənbə kitabları, məqalə mətnləri və səs yazıları bu repoya köçürülməyib; onların
müəlliflik hüquqları sahiblərində qalır. Bu skill rəsmi akademik nəşr deyil.
