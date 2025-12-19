# SpiderFoot Local OSINT Project

## Proje Nedir?

Bu proje, açık kaynaklı **SpiderFoot** OSINT (Open Source Intelligence) aracının **lokal ortamda** kurulup çalıştırılmasını amaçlayan bir çalışmadır. SpiderFoot; IP adresi, domain, e‑posta, telefon numarası, kullanıcı adı gibi verilerden otomatik olarak açık kaynaklardan bilgi toplamaya yarar.

Bu repo; kurulumu, bağımlılıkları ve temel kullanım adımlarını sade şekilde göstermek için hazırlanmıştır.

> ⚠️ **Yalnızca eğitim ve araştırma amaçlıdır. İzinsiz ve hukuka aykırı kullanım sorumluluğu kullanıcıya aittir.**

---

## Gereksinimler

* Python **3.7+**
* pip
* Git (opsiyonel)

---

## Kurulum Adımları

### 1️⃣ Repoyu indirin

```bash
git clone https://github.com/USERNAME/spiderfoot-local.git
cd spiderfoot-local
```

Ya da ZIP olarak indirip klasöre girin.

---

### 2️⃣ Gerekli Python kütüphanelerini yükleyin

```bash
pip install -r requirements.txt
```

Eğer eksik modül hataları alırsanız aşağıdaki temel kütüphaneleri manuel kurabilirsiniz:

```bash
pip install python-docx
pip install python-pptx
pip install ipwhois
pip install python-whois
pip install requests
pip install beautifulsoup4
pip install lxml
```

---

### 3️⃣ SpiderFoot Web Arayüzünü Başlatın

```bash
python sf.py -l 127.0.0.1:5001
```

Tarayıcıdan açın:

```
http://127.0.0.1:5001
```

---

## Nasıl Kullanılır?

### Yeni Tarama (Scan) Oluşturma

1. Web arayüzünde **New Scan** seçin
2. Elinizdeki veri tipini girin
3. Uygun modülleri seçin
4. Scan’i başlatın

---

## Elinizde Ne Varsa Ne Bulabilirsiniz?

### 📱 Telefon Numarası

* Ülke ve operatör bilgisi
* Veri sızıntılarında (leak) geçip geçmediği
* Diğer kaynaklarda tekrar eden kullanımlar

> ❗ Telefon numarasından **doğrudan Instagram hesabı bulunmaz**

---

### 📧 E‑posta Adresi

* Veri ihlallerinde yer alıp almadığı
* Sosyal medya hesapları
* Kullanıcı adları
* İlişkili domainler

---

### 👤 Kullanıcı Adı (Username)

* Instagram, Twitter, GitHub, Reddit vb. platformlar
* Aynı kullanıcı adının geçtiği diğer siteler

---

### 🌐 Domain / Website

* Alt domainler
* E‑posta adresleri
* Sunucu bilgileri
* Açık dosyalar
* Teknoloji altyapısı

---

### 🌍 IP Adresi

* Lokasyon
* ASN
* Açık portlar
* Kara listeler
* İlişkili domainler

---

## Önemli Notlar

* Bazı modüller **API key** ister
* Sosyal medya sonuçları sınırlı olabilir
* Leak sonuçları her zaman çıkmayabilir
* Telefon numarası OSINT’te en zor veri tipidir

---

## Kimler İçin Uygun?

* OSINT öğrenmek isteyenler
* Siber güvenliğe giriş yapanlar
* Python tabanlı araçları kurup çalıştırmak isteyenler

---

## Lisans

SpiderFoot MIT lisansı ile dağıtılmaktadır.
Bu repo eğitim amaçlıdır.
