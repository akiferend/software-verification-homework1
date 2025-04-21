# BankingApp3

**BankingApp3**, bir JavaFX tabanlı bankacılık uygulamasıdır. Uygulama, müşteri ve hesap yönetimi gibi temel bankacılık işlemlerini gerçekleştirmek için tasarlanmıştır.

## 🚀 Özellikler

- **Müşteri Yönetimi**: Müşteri bilgilerini ekleme, güncelleme, silme ve görüntüleme.
- **Hesap Yönetimi**: Hesap bilgilerini ekleme, güncelleme, silme ve görüntüleme.
- **Veritabanı Bağlantısı**: PostgreSQL kullanılarak müşteri ve hesap bilgileri saklanır.
- **JavaFX Arayüzü**: Kullanıcı dostu bir grafik arayüz.

## 📦 Gereksinimler

- **Java 17** veya daha üstü  
- **Maven** (Proje bağımlılıklarını yönetmek için)  
- **PostgreSQL** (Veritabanı)

## ⚙️ Kurulum

### 1. Projeyi Klonlayın

```bash
git clone https://github.com/kullaniciadi/BankingApp3.git
cd BankingApp3
```

### 2. Gerekli Bağımlılıkları Yükleyin

```bash
./mvnw clean install
```

### 3. PostgreSQL Veritabanınızı Yapılandırın

- **Veritabanı adı**: `banking_db`  
- **Kullanıcı adı**: `gorkemdb`  
- **Şifre**: `gorkemdb`

Aşağıdaki SQL komutlarını çalıştırarak tabloları oluşturun:

```sql
CREATE TABLE Customers (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100),
    address VARCHAR(255),
    city VARCHAR(100)
);

CREATE TABLE Account (
    id SERIAL PRIMARY KEY,
    branch VARCHAR(100),
    balance NUMERIC(15, 2)
);
```

### 4. Uygulamayı Çalıştırın

```bash
./mvnw javafx:run
```

## 🧑‍💼 Kullanım

- **Müşteri Yönetimi**: Müşteri bilgilerini eklemek, güncellemek, silmek veya görüntülemek için müşteri arayüzünü kullanabilirsiniz.  
- **Hesap Yönetimi**: Hesap bilgilerini eklemek, güncellemek, silmek veya görüntülemek için hesap arayüzünü kullanabilirsiniz.

## 🤝 Katkıda Bulunma

Katkıda bulunmak isterseniz, lütfen bir **pull request** gönderin veya bir **issue** açın.

## 📄 Lisans

Bu proje [Apache 2.0 Lisansı](https://www.apache.org/licenses/LICENSE-2.0) ile lisanslanmıştır.
```
