MOOM 8.6 - AYRI AK-47 / SNIPER MODELLERI VE 3 YENI ACIK HAVA BOLUMU

BU SURUMDE
- AK-47 artik M249 modelini kullanmiyor; kendine ait 3D govde, namlu, el korumasi, sarjor ve dipcik modeline sahip.
- Sniper artik M249 modelini kullanmiyor; kendine ait uzun namlu, govde, optik nisangah ve dipcik modeline sahip.
- Silah degistirme sirasi: Shotgun, Dual Pistols, M249, Crowbar, Grenade Launcher, AK-47, Sniper.
- Sniper durbun kontrolleri: Asagi tusu durbun modunu acar/kapatir; Kare yakinlastirir, Yuvarlak uzaklastirir.
- Iki yeni bolum eklendi:
  8. Terk Edilmis Liman
  9. Metro Istasyonu
- Bolum secim ekrani 9 bolumu gosterecek sekilde siklastirildi.
- Onceki MOOM ozellikleri, menuler, sesler, bombaatar patlama efekti ve onceki 7 bolum korunmustur.

KONTROLLER
- Ana menu: Yukari/Asagi secim, X veya START onay
- Bolum secimi: Yukari/Asagi gezinme, X veya START baslatma, O geri
- Ayarlar: Yukari/Asagi satir secimi, X secenegi degistir, O geri
- Oyun: Analog/yon tuslari hareket ve donus; L1 yana yurume; R1 silah degistir; X/Kare silah kullan
- Sniper: Asagi durbun; durbun acikken Kare yakinlastir, Yuvarlak uzaklastir, X ates

DERLEME
main.c ve Makefile dosyalarini PSP SDK projenize koyup PSPSDK ile EBOOT.PBP derleyin.

DOGRULAMA
Kaynak kodda yeni model olusturma/cizim cagrilari, bolum tanimlari ve bolum secim araligi kontrol edildi.
Bu ortamda PSP SDK (psp-config / psp-gcc) bulunmadigindan PSP derlemesi ve PPSSPP uzerinde calisma testi yapilmadi.
Bu nedenle derlenmis EBOOT.PBP veya calisma garantisi sunulmuyor.

INCELEME NOTU
- Ilk 8.3 ZIP'indeki LV7_ROWS ve LV8_ROWS tanimlarinda satir sonlari gercek satir sonu yerine literal \\n karakterleri olarak yazilmisti; bu C derlemesini bozabilirdi.
- Bu duzeltilmis pakette bu iki bolum tanimi normal C satirlarina ayrildi.


MOOM 8.6 - 3 yeni acik hava bolumu:
10. SEHIR PARKI - genis acik alan, park duvarlari ve acik gokyuzu.
11. KASABA DISI - terk edilmis kasaba cevresi ve acik yollar.
12. ORMAN YOLU - acik orman yolu ve daginik engeller.
Bu uc bolumde tavan geometrisi cizilmez; acik gokyuzu, daha aydinlik ortam ve renkli sis kullanilir.
Bolum secim ekrani 12 bolumu PSP ekranina sigdirmak icin kayan listeye donusturuldu.

PPSSPP GORUNEN SURUM ADI
- Makefile icindeki PSP_EBOOT_TITLE alani MOOM 8.6 olarak ayarlanmistir.
- Yeni EBOOT.PBP dosyasini bu Makefile ile yeniden derleyin; eski EBOOT.PBP dosyasinin adi degismez.


MOOM 8.6 - MUSTI NORMAL ZOMBI DOKUSU
- Kullanıcının sağladığı, yüzü siyah sansürlü tam boy fotoğraf arka plandan ayrıştırılarak 64x64 RGBA sprite dokusuna dönüştürüldü.
- Bu doku normal zombi türünün tamamında kullanılır; özel boss değildir.
- Ölüm dokusu mevcut siyah ceset sisteminden oluşturulmaya devam eder.
- PSP SDK derlemesi ve PPSSPP testi bu ortamda yapılmadı.


KONTROL SONRASI DUZELTME
- Makefile icindeki PSP_EBOOT_TITLE MOOM 8.6 olarak guncellendi.
- main.c dosyasinin surum yorumu MOOM 8.6 olarak guncellendi.
- MUSTI dokusu 64x64 (4096 piksel) olarak kontrol edildi ve normal zombi dokusuna bagli.


MOOM 8.6 - UZAKTAN SALDIRAN ZOMBI GORUNUMU
- Uzaktan saldiran zombi (tip 1 / S) artik kullanicinin ikinci fotografindan uretilen 64x64 RGBA sprite dokusunu kullanir.
- Normal zombi (tip 0 / Z) onceki MUSTI fotograf dokusunu kullanmaya devam eder.
- Uzaktan saldiran zombinin mevcut saldiri/yapay zeka davranisi degistirilmedi.
- Uzaktan saldiran sprite daha dar ve uzun cizilir; diger dusman turlerinin boyutlari korunur.
- PSP SDK ile derleme ve PPSSPP testi bu ortamda yapilmadi.


MOOM - TITAN ASKERI KARGO UCAGI TAHLIYE SISTEMI
- Ucak haritaya yaklasip piste/duz alana iner.
- Pervaneler doner, arka rampa acilir ve tahliye geri sayimi baslar.
- Oyuncu arka rampaya girerse gorev tamamlanir; sure biterse rampa kapanip kalkis yapar ve gorev basarisiz olur.
- Mevcut silah, zombi, harita ve ses yapilari korunmustur.
