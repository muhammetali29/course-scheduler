# Kurs Planlayıcı

Bu, okulunuz için kolayca bir ders programı oluşturmanıza olanak sağlayan bir web uygulamasıdır.

## Ekran Görüntüleri

<img src="/screenshots/Screenshot 1.png" width="600"/>
<img src="/screenshots/Screenshot 2.png" width="600"/>
<img src="/screenshots/Screenshot 3.png" width="600"/>

## Başlarken

### Önkoşullar

- [Node.js](https://nodejs.org/en/)
- [PostgreSQL](https://www.postgresql.org/)

### Installing

Depoyu bilgisayarınıza klonlayın.

```bash
git clone https://github.com/aydinkasimoglu/course-scheduler.git
```

Gerekli bağımlılıkları yükleyin.

```bash
cd course-scheduler
npm install
```
### Yapılandırma

Projenin kök dizininde bir `.env` dosyası oluşturun ve aşağıdaki değişkeni ekleyin.

```conf
DATABASE_URL="postgresql://<username>:<password>@localhost:5432/<db_name>"
```

### Migration

Veritabanı tablolarını oluşturmak için migrasyon işlemi çalıştırılmalıdır. Bu projede ORM aracı olarak Prisma (https://www.prisma.io/
) kullanılmaktadır.

```bash
npx prisma migrate dev
```

### Çalıştırma

Geliştirme sunucusunu çalıştırın. Sunucu varsayılan olarak 3000 numaralı bağlantı noktasında çalışacaktır.

```bash
npm run dev
```

