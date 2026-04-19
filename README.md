# 📅 LinkedIn Scheduler

LinkedIn postlarını planlamak, düzenlemek ve yönetmek için geliştirilmiş **lokal çalışan** bir web uygulaması.

Sunucu yok. Abonelik yok. Veriler tamamen sende.

---

## Neden yaptım?

LinkedIn'in yerleşik planlama özelliğini kullanıyordum. Güzel gidiyordu — ta ki araya yeni bir post sokmam gerekene kadar. Yeni postu ilk sıraya almak istiyorum, yani önceki tüm postları elle kaydırmam gerekiyor. 10 post × elle düzenleme = sinir bozucu.

Excel'e geçtim, formül kurdum, olmadı. Sonra kendime sordum: Ben bilgisayar mühendisiyim, neden kendi sistemimi kurmayayım?

---

## Özellikler

- **Post yönetimi** — Oluştur, düzenle, sil, kopyala
- **Durum takibi** — Taslak / Planlanmış / Bugün / Geçmiş / Paylaşıldı
- **Medya desteği** — Birden fazla fotoğraf veya video ekle
- **Zincir kaydırma** — Bir postu kaydır, sonraki tüm postlar otomatik kayar
- **Takvim görünümü** — Postları takvimde sürükle-bırak ile taşı
- **Otomatik JSON kayıt** — Her değişiklik anında `posts.json` dosyasına yazılır
- **İstatistik paneli** — Toplam, planlanmış, bugün, paylaşıldı sayaçları
- **Import / Export** — JSON olarak yedekle veya geri yükle
- **Tamamen lokal** — İnternet bağlantısı gerektirmez

---

## Kurulum

Herhangi bir kurulum gerektirmez.

1. `linkedin-scheduler.html` dosyasını indir
2. Çift tıkla, tarayıcıda aç
3. Kullanmaya başla

> Chrome veya Edge önerilir (File System API desteği için)

---

## Nasıl çalışır?

```
Scheduler (HTML)  →  posts.json  →  n8n  →  Bildirim (E-posta + Masaüstü)
```

Uygulama, postları `posts.json` dosyasına kaydeder. n8n her sabah bu dosyayı okur, o güne ait planlanmış postları bulur ve sana bildirim gönderir.

---

## Teknolojiler

- **HTML / CSS / JavaScript** — Tek dosya, sıfır bağımlılık
- **File System Access API** — Tarayıcıdan doğrudan diske yazma
- **IndexedDB** — Klasör bağlantısını hatırlama
- **localStorage** — Post verilerini saklama

---

## Ekran Görüntüleri

> Yakında eklenecek

---

## Lisans

MIT — dilediğin gibi kullan, değiştir, dağıt.
