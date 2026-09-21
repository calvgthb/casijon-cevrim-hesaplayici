# Casijon Çevrim Şartı Hesaplayıcı

Casijon bonus kampanyalarında **çevrim şartını** hesaplayan basit bir web aracı.
Bağımlılık yok, tek HTML dosyası, tarayıcıda çalışır.

**Canlı sürüm:** https://calvgthb.github.io/casijon-cevrim-hesaplayici/

---

## Ne işe yarar

Bonus alan kullanıcıların en sık takıldığı konu çevrim şartı. "500 TL bonus
aldım, ne kadar bahis yapmam gerekiyor?" sorusunun cevabı üç değişkene bağlı:

- Bonus tutarı
- Çevrim katsayısı (10x, 20x gibi)
- Oynanan oyunun katkı oranı (slot %100, canlı casino %50 gibi)

Bu araç üçünü birleştirip gereken toplam bahis tutarını veriyor.

## Çevrim şartı nasıl hesaplanır

Çevrim şartı, bonusun çekilebilir bakiyeye dönüşmesi için yapılması gereken
**toplam bahis** tutarıdır. Kazanç değil, bahislerin toplamı.

```
gereken bahis = taban × katsayı × (100 / katkı oranı)
```

### Örnek

500 TL bonus, 10x çevrim, %100 katkılı slot:

```
500 × 10 × (100/100) = 5.000 TL
```

Aynı bonus %50 katkılı canlı casinoda:

```
500 × 10 × (100/50) = 10.000 TL
```

Katkı oranı düştükçe gereken bahis artar. Bu yüzden hangi oyunda çevirdiğiniz
önemli.

### Katkı oranı karşılaştırması

| Oyun türü | Tipik katkı | 500 TL / 10x için gereken |
|---|---|---|
| Slot | %100 | 5.000 TL |
| Canlı casino | %50 | 10.000 TL |
| Masa oyunları | %20 | 25.000 TL |

## Sık yapılan hata

Çevrim tamamlanmadan çekim talebi açmak. Bu durumda bonus bakiyesi ve
bonustan elde edilen kazanç iptal edilir; yalnızca kendi yatırdığınız tutar
kalır. Bu bir ceza değil, kampanyanın baştan yazılı olan kuralıdır.

## Kurulum

Dosyayı indirip tarayıcıda açmanız yeterli:

```
git clone https://github.com/calvgthb/casijon-cevrim-hesaplayici.git
cd casijon-cevrim-hesaplayici
```

`index.html` dosyasını çift tıklayın. Sunucu, derleme veya bağımlılık gerekmez.

## Katkı

Hata bildirimi ve öneriler için issue açabilirsiniz.

## Casijon hakkında

Casijon; spor bahisleri, canlı casino ve slot oyunlarını tek platformda sunan
çevrimiçi bahis ve casino markasıdır.

- **Web:** [casijon.net](https://casijon.net/)
- **Bonus kampanyaları:** [casijon.net/bonuslar](https://casijon.net/bonuslar/)
- **Sık sorulan sorular:** [casijon.net/sss](https://casijon.net/sss/)
- **Telegram:** [t.me/s/casijon](https://t.me/s/casijon)
- **Instagram:** [@casijonresmi](https://www.instagram.com/casijonresmi/)

> Bu araçtaki oranlar örnek amaçlıdır. Geçerli çevrim katsayısı ve katkı
> oranları kampanyaya göre değişir; işlem yapmadan önce Casijon bonus
> şartlarını kontrol edin.

## Sorumlu oyun

18 yaşından küçükler oynayamaz. Şans oyunları gelir kaynağı değildir.
Oynamadan önce bütçe ve süre sınırı belirleyin, kaybettiğinizi geri kazanmak
için bahis artırmayın.

## Lisans

MIT
