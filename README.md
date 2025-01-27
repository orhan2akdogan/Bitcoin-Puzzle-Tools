# Bitcoin Puzzle Çözüm Araçları Rehberi 🧩

Bu rehber, Bitcoin puzzle'larını çözmek için kullanılan popüler araçları karşılaştırır ve hangi senaryolarda tercih edileceklerini açıklar.

---

## 📊 Araç Karşılaştırma Tablosu

| Araç               | Donanım        | Temel Özellikler                                                                 | Kullanım Senaryosu                          | Artılar                                      | Eksiler                                       | Bağlantılar                                   |
|--------------------|---------------|---------------------------------------------------------------------------------|---------------------------------------------|---------------------------------------------|----------------------------------------------|-----------------------------------------------|
| **Keyhunt**        | 🖥️ CPU        | BSGS algoritması, yüksek RAM kullanımı                                          | #66+ büyük puzzle'lar (CPU sınırlı)         | Geniş keyspace taraması                     | GPU yok, yavaş                               | [GitHub](https://github.com/albertobsd/keyhunt) |
| **Keyhunt-CUDA**   | 🎮 NVIDIA GPU  | Keyhunt'un CUDA destekli versiyonu, yüksek hız                                   | #70+ dev puzzle'lar                         | Bitcrack'ten %30 hızlı, çoklu GPU           | Kurulum karmaşık                            | [GitHub](https://github.com/kanhavishva/keyhunt-cuda) |
| **Bitcrack**       | 🎮 NVIDIA GPU  | Temel brute-force, manuel multi-GPU                                             | Küçük aralıklar (#50-65)                    | Basit kullanım                              | İlerleme takibi yok, düşük verim             | [GitHub](https://github.com/brichard19/BitCrack) |
| **Kangaroo**       | 🖥️ CPU/GPU    | Pubkey tabanlı arama, Pollard's Kangaroo algoritması                            | Pubkey bilinen adresler                     | Büyük keyspace'lerde etkili                 | Pubkey gerekliliği                           | [GitHub](https://github.com/JeanLucPons/Kangaroo) |
| **BSGS-CUDA**      | 🎮 NVIDIA GPU  | BSGS'in CUDA destekli versiyonu                                                 | Orta ölçekli puzzle'lar (#50-70)            | Hızlı tarama                                | PureBasic v5.3 gereksinimi                   | [GitHub](https://github.com/Etayson/BSGS-CUDA) |
| **Brainflayer**    | 🖥️ CPU/GPU    | Brainwallet brute-force, kelime listesi desteği                                 | Brainwallet tahmini                         | Esnek giriş formatı                         | Yüksek RAM tüketimi                          | [GitHub](https://github.com/ryancdotorg/brainflayer) |
| **VanBitCracken**  | 🎮 NVIDIA GPU  | Nvidia 3070 optimizasyonu, rastgele/sekans modları                              | Windows tabanlı çözümler                    | Kullanıcı dostu arayüz                      | Kaynak kodu kapalı (riskli)                  | [Forum](https://bitcointalk.org/index.php?topic=1306983.0) |

---

## 🎯 Kullanım Senaryoları

### 1. **Büyük Puzzle'lar (#70+)**  
- **Önerilen Araç:** `Keyhunt-CUDA` (yüksek hız) veya `Rotor-CUDA` (esneklik).  

### 2. **Pubkey Bilinen Adresler**  
- **Önerilen Araç:** `Kangaroo` (algoritmik avantaj).  

### 3. **Brainwallet Tahmini**  
- **Önerilen Araç:** `Brainflayer` (kelime listeleri ile optimize).  

### 4. **Küçük Aralıklar (#1-50)**  
- **Önerilen Araç:** `BSGS` (CPU verimliliği) veya `Bitcrack` (basitlik).  

---

## ⚠️ Önemli Uyarılar
- **Güvenlik:** `VanBitCracken` gibi kaynak kodu kapalı araçları kullanırken dikkatli olun. Resmi bağlantılar dışındaki dosyaları çalıştırmayın.
- **Performans:** GPU araçları (Keyhunt-CUDA, Bitcrack) NVIDIA kartlarıyla en iyi verimi alır.
- **Güncellemeler:** `BSGS-CUDA` gibi eski araçların sürüm uyumluluğunu kontrol edin.

---

## 🔗 Faydalı Bağlantılar
- [Bitcoin Puzzle Çözüm Forumu](https://bitcointalk.org)
- [CUDA Kurulum Rehberi](https://developer.nvidia.com/cuda-downloads)
