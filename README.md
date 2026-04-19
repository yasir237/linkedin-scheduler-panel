# 📅 LinkedIn Scheduler - Panel

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

<img width="1919" height="907" alt="Ekran görüntüsü 2026-04-19 180552" src="https://github.com/user-attachments/assets/af40ff95-67cb-4cba-b415-11424711a1a6" />

---

<img width="1919" height="910" alt="Ekran görüntüsü 2026-04-19 175048" src="https://github.com/user-attachments/assets/6217bd68-ddd0-4d7d-a7a4-cfe267ffb370" />

---

<img width="1919" height="905" alt="Ekran görüntüsü 2026-04-19 175100" src="https://github.com/user-attachments/assets/ac74ff75-e439-464a-a34a-dde01f0004da" />

---

<img width="1919" height="901" alt="Ekran görüntüsü 2026-04-19 175222" src="https://github.com/user-attachments/assets/77b321b8-c32d-4911-96f4-78da468a41a7" />


---

## Lisans

MIT — dilediğin gibi kullan, değiştir, dağıt.
