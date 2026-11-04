# Jaya Player — qo‘llanma

Jaya Player — Android TV, TV-pristavkalar va smartfonlar uchun IPTV-pleyer.
Dastur **telekanallar va kontent taqdim etmaydi**: u faqat foydalanuvchi o‘zi qo‘shgan pleylistlarni ijro etadi.

---

## 1. O‘rnatish

1. Dasturni yuklab oling: **https://github.com/FirstRandomUser/jaya-player-releases/releases/latest/download/jaya-player.apk** (doim eng so‘nggi versiya) yoki [Releases](https://github.com/FirstRandomUser/jaya-player-releases/releases/latest) sahifasidan.
2. TV-pristavkada **Downloader** ilovasi yoki fleshka qulay.
3. Birinchi o‘rnatishda Android ushbu manbadan o‘rnatishga ruxsat so‘raydi — ruxsat bering.
4. Android 6.0 yoki undan yangisi talab qilinadi.

Keyingi yangilanishlarni dastur **o‘zi** yuklab, o‘rnatadi (10-bo‘limga qarang).

---

## 2. Birinchi ishga tushirish va pleylist

Birinchi ishga tushirishda **Sozlamalar** ochiladi.

1. **Pleylistlar → Qo‘shish** tugmasini bosing.
2. Turini tanlang:
   - **M3U havolasi** — provayder bergan pleylist manzili;
   - **Xtream Codes** — server manzili, login va parol;
   - **fayl** — qurilmadagi yoki fleshkadagi `.m3u` pleylist.
3. **EPG** (ko‘rsatuvlar dasturi) — XMLTV manzili. Odatda u provayder pleylistida bor, maydonni bo‘sh qoldirish mumkin. Ko‘rsatuvlar dasturi bo‘lmasa, EPG manzilini provayderingizdan bilib, shu yerga yozing.
4. **Har … soatda yangilash** — pleylist va ko‘rsatuvlar dasturi qanchalik tez-tez yangilanishi.
5. **Saqlash** tugmasini bosing. Yuklash fonda boradi — darhol tomoshaga qaytishingiz mumkin.

Bir nechta pleylist qo‘shish mumkin. Yangilash xato bilan tugasa (masalan, internet bo‘lmasa), dastur keyingi ishga tushirishda uni o‘zi takrorlaydi.

---

## 3. Pult bilan boshqarish

| Tugma | Amal |
|---|---|
| ▲ ▼ | oldingi / keyingi kanal |
| ◀ | kanallar ro‘yxati |
| ◀ ◀ (yana chapga) | guruhlar ro‘yxati |
| ▶ | Sevimlilar |
| ▶ ▶ (ikki marta tez) | oqim statistikasi (yoqish/o‘chirish) |
| OK | ma’lumot paneli |
| yana OK | pauza |
| pauzada OK | davom ettirish |
| uzoq OK | amallar menyusi (ovoz, subtitr, format, sozlamalar) |
| raqamlar | raqam bo‘yicha kanalga o‘tish |
| 0 | oldingi kanal |
| ikki marta «Orqaga» | chiqish |

**Kanallar ro‘yxatida:**
- ▶ — tanlangan kanalning ko‘rsatuvlar dasturi;
- uzoq OK — belgilash rejimi: ◀ Sevimlilarga qo‘shish/olib tashlash, ▶ kanalni o‘chirish (o‘chirilganlarni «O‘chirilganlar» guruhidan qaytarish mumkin).

**Smartfonda:** teginish — pauza va ma’lumot paneli; yuqoriga surish — panel, pastga — yashirish; ekranning chap yarmida o‘ngga surish — kanallar ro‘yxati; o‘ng yarmida chapga — Sevimlilar; uzoq teginish — sozlamalar.

---

## 4. Ko‘rsatuvlar dasturi va arxiv

- Ko‘rsatuvlar dasturi **24 soat orqaga va 48 soat oldinga** saqlanadi.
- Kanallar ro‘yxatida ▶ bosing — ko‘rsatuvlar dasturi ochiladi. Provayder qo‘llab-quvvatlasa, o‘tgan ko‘rsatuvlarni **arxivdan** ko‘rish mumkin.
- Arxivda: **OK** — o‘tkazish chizig‘i, ◀ ▶ — qadam (bosib tursangiz tezlashadi), **Orqaga** — jonli efirga qaytish.

---

## 5. Efirni pauza qilish (Timeshift)

**Sozlamalar → Ijro → Yozuv bilan efirni pauza qilish.**

- **O‘chiq:** pauza tasvirni to‘xtatadi; davom ettirilganda — jonli efir.
- **Yoqiq:** pauzadan keyin tomosha **aynan o‘sha joydan** davom etadi. Efirdan orqada qolish pastda ko‘rinadi; **Orqaga** — efirga qaytish.

**Pauza yozuvi xotirasi:**
- **Ichki xotira** — yozuv pauza paytida boshlanadi va kanal almashtirilganda o‘chiriladi.
- **Tashqi disk (fleshka)** — kanalni ko‘rayotganingizda yozuv doim boradi, shuning uchun **pauzada ◀ ▶ orqaga o‘tkazadi** (joy yetgunicha). Dastur fleshkada `Timeshift` papkasini yaratadi va bo‘sh joyning ko‘pi bilan 80 % ini ishlatadi; eski yozuvlar avtomatik o‘chiriladi.

Fleshka: FAT32 yoki exFAT (qurilmangiz qo‘llasa — NTFS).
DASH oqimlari, shifrlangan oqimlar va alohida ovoz yo‘lakli oqimlar qo‘llab-quvvatlanmaydi — ularda pauza odatdagidek ishlaydi.

---

## 6. Yashirin guruhlar (ota-ona nazorati)

1. Guruhlar ro‘yxatini oching (◀ ◀), guruhni tanlang va **OK ni bosib turing** — guruhlarni tanlash yoqiladi.
2. Guruhlarni OK bilan belgilang va **Orqaga** bosing.
3. Parolni strelkalar bilan kiriting va OK bosing. Standart parol — **▶ ▶ ▶ ▶**.
4. Birinchi yashirishdan keyin dastur strelkalardan o‘z parolingizni o‘ylab topishni taklif qiladi (masalan ▲ ▲ ◀ ▶) — uni eslab qoling.

Yashirin guruhlarni qayta ko‘rsatish uchun guruhlar ro‘yxatida **◀ ni uch marta tez bosing** va parolni kiriting. Dastur yig‘ilganda guruhlar yana yashiriladi.

---

## 7. Rasm ichida rasm va fon (smartfon)

- **Rasm ichida rasm:** bosh ekranga chiqqanda video kichik oynada davom etadi.
- **Fonda ovoz:** ekran qulflanganda ovoz davom etadi; boshqaruv — bildirishnomalar panelidan.

---

## 8. Sozlamalar

- **Ekran:** kadr chastotasini avtomatik almashtirish, 120 Gs, ma’lumot paneli ko‘rinish vaqti, ro‘yxatlarni aylantirish, **OLED ekran** (kuyishdan himoya: elementlarni siljitish, soatni yashirish, pauzada ekran saqlovchi, menyuni xiralashtirish).
- **Soat:** ekrandagi o‘rni.
- **Ijro:** rasm ichida rasm, fonda ovoz, ovoz balandligini tenglash, statistika, efir pauzasi, qo‘shni kanallarni oldindan yuklash, bufer, User-Agent.
- **Mavzular** (sozlamalardagi alohida «Mavzular» tugmasi): tayyor mavzular (Klassik, OLED qora, Okean, Iliq, Shisha) yoki panellar, tanlov, matn, ma’lumot paneli, soatning o‘z ranglari va shaffoflik.
- **Ma’muriyat:** parol va sozlama bandlarini qulflash (qulflangan bandlar yashiriladi).

**User-Agent** — pleyer provayder serveriga o‘zini qanday «tanishtirishi». Pleylist yuklansa-yu, kanallar ochilmasa — **VLC** ni sinab ko‘ring.

---

## 9. Zaxira nusxa

**Sozlamalar → Ilova haqida → Eksport** pleylistlar, Sevimlilar, yashirin guruhlar va sozlamalarni faylga saqlaydi. **Import** ularni tiklaydi — masalan, yangi qurilmada.

---

## 10. Yangilanishlar

- Dastur yangilanishlarni o‘zi tekshiradi, yuklaydi va o‘rnatadi (**Ilova haqida** bo‘limida o‘chirish mumkin).
- O‘rnatishdan oldin imzo tekshiriladi — yangilanishni soxtalashtirib bo‘lmaydi.
- Dastur **90 kun** davomida yangilanishni tekshira olmasa, cheklangan rejim yoqiladi (ko‘rsatuvlar dasturi va arxivsiz, Sevimlilarda 5 kanal). Internetga ulanish kifoya — hammasi qaytadi.

---

## 11. Pro versiya

Hozir barcha imkoniyatlar **bepul**. Pro chiqqanda har kimga yana **3 oy** to‘liq kirish beriladi.

| | Bepul | Pro |
|---|---|---|
| Sifat | 1080p gacha (4K/HDR — 3 daqiqa) | 4K, HDR |
| Sevimlilar | 20 kanal | cheklovsiz |
| Yashirin guruhlar | 1 | cheklovsiz |
| Arxiv | oxirgi 3 soat | provayder bergancha |
| Ovozni tenglash, kadr chastotasini avtomatik almashtirish, 120 Gs, resiverga AC3/DTS | — | ✓ |
| Yozuv bilan efir pauzasi, mavzular | — | ✓ |
| Rasm ichida rasm va fonda ovoz (smartfon) | — | ✓ |

---

## 12. Biror narsa ishlamasa

- **Kanal ochilmaydi** — User-Agent ni almashtiring (VLC); pleylistni boshqa qurilmada tekshiring.
- **Ko‘rsatuvlar dasturi yo‘q** — pleylistdagi EPG manzilini tekshiring; **Pleylistlar** bo‘limini oching — yuklash xatosi o‘sha yerda ko‘rinadi.
- **Smartfonda ovozni tenglashda ovoz xirillaydi** — tenglashni o‘chiring.
- **Kuchsiz pristavkada 4K to‘xtab-to‘xtab ketadi** — «Katta» buferni tanlang yoki HD da ko‘ring.

---

## 13. Qurilmalarni ulash va sifat

- **Qurilmalarni ulash** (Sozlamalar → Qurilmalarni ulash): telefonni televizorga kod bilan ulang — kod TV ekranida o‘zi chiqadi. Pleylistlar va sozlamalarni yuborish, QR orqali brauzerdan pleylist qo‘shish, telefondan TV ga uzatish (📺, telefon pultga aylanadi) va tomoshani qaytarib olish.
- **Sifat** (ma’lumot paneli): «Avto» sekin tarmoqda sifatni pasaytiradi; «Eng yaxshi» — doim eng yuqori. Har bir kanal uchun eslab qolinadi.
- **«Avto» bufer**: tez-tez to‘xtasa, bufer o‘zi kattalashadi.

---

## 14. Qulaylik

- **Eslatmalar:** dasturda kelajakdagi ko‘rsatuvga OK — ◉ belgisi, boshlanishidan bir daqiqa oldin «O‘tish» oynasi chiqadi.
- **Sevimlilar:** uzoq OK — ▲▼ tartibini o‘zgartiradi, OK nomini o‘zgartiradi.
- **Ekrandagi dastur**, **interfeys o‘lchami**, **avtoishga tushish**, yangi **«Neon»** mavzusi.

---

© 2026 Ruslan G. Barcha huquqlar himoyalangan.
