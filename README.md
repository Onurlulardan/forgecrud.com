# ForgeCRUD

ForgeCRUD, yazılım geliştiricilere yönelik olarak veritabanı tasarımı, API rotaları ve yönetim paneli oluşturma süreçlerini kolaylaştıran bir platformdur. Bu proje, kullanıcıların veritabanı şemalarını oluşturup, otomatik olarak Next.js tabanlı projeler için API rotaları ve Chakra UI ile özelleştirilmiş bir yönetim paneli oluşturmalarını sağlar.

## Özellikler

- **Veritabanı Tasarımı**: React Flow kullanarak 1:1, 1:N ve N:N ilişkilerle veritabanı diyagramları oluşturma.
- **API Rotaları**: Veritabanı diyagramına dayalı olarak otomatik API rotası oluşturma.
- **Otomatik Yönetim Paneli**: Chakra UI ile özelleştirilebilir yönetim paneli.
- **Deploy İşlevi**: Tek tıklamayla şema ve API rotalarını konuşlandırma.
- **Prisma Şema Yönetimi**: Prisma desteğiyle SQL çıktısını görüntüleyebilme.
- **Analitik Takip**: Ackee entegrasyonu ile kullanıcı aktivitelerini izleme (buton tıklamaları vb.).
- **Rate Limiting**: Özel API uç noktaları için güvenli erişim ve hız sınırlaması.

## Kurulum

### Gereksinimler

- Node.js ve npm
- Prisma CLI
- Ackee (analitik için)
- Docker (isteğe bağlı, Ackee veya veritabanı yapılandırması için)

### Adımlar

1. **Depoyu klonlayın**:
    ```bash
    git clone https://github.com/kullanici-adiniz/ForgeCRUD.git
    cd ForgeCRUD
    ```

2. **Bağımlılıkları yükleyin**:
    ```bash
    npm install
    ```

3. **.env dosyasını oluşturun**:
   `.env` dosyasını projenin kök dizinine ekleyin ve örnek `.env.example` dosyasındaki gerekli bilgileri doldurun.

4. **Veritabanı ve Prisma kurulumunu yapın**:
    ```bash
    npx prisma migrate dev
    ```

5. **Geliştirme sunucusunu başlatın**:
    ```bash
    npm run dev
    ```

ForgeCRUD artık `http://localhost:3000` adresinde çalışacaktır.

## Kullanım

1. **Veritabanı Tasarımı**: 
   - React Flow arayüzünü kullanarak tablolar ve ilişkiler oluşturun.
   - Farklı ilişki türleri (1:1, 1:N, N:N) ekleyebilirsiniz.

2. **API Rotası ve Yönetim Paneli**:
   - Tasarım tamamlandığında "Deploy" düğmesine basarak API rotaları ve yönetim panelini otomatik olarak oluşturun.
   - Yönetim paneli Chakra UI kullanılarak oluşturulmuştur ve özelleştirilebilir bileşenler içerir.

3. **Analitik Takip**:
   - Ackee ile entegrasyonu etkinleştirerek kullanıcı davranışlarını takip edin.
   - Buton tıklamaları gibi belirli eylemleri izleyebilir ve analiz edebilirsiniz.

## Yapılacaklar

- Kullanıcı profillerine yönelik genişletilmiş alanlar (profesyonel bilgiler, iş unvanı vb.).
- Veri görselleştirme araçları ve gelişmiş analitik entegrasyonları.
- Daha fazla veritabanı destekleyebilmek için uyumluluk güncellemeleri.

## Katkıda Bulunun

Katkıda bulunmak isteyen geliştiriciler, projeyi fork ederek geliştirme yapabilir. Herhangi bir öneri veya hata bildirimi için lütfen bir **pull request** veya **issue** açın.

## Lisans

Bu proje [MIT Lisansı](LICENSE) ile lisanslanmıştır.

---

Bu belgede eksik olduğunu düşündüğün herhangi bir şey varsa eklemeler yapabiliriz!
