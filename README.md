# Rest-API-Golang
It is a rest api project that will perform crud operations in golang language.

## Getting Started

### Projeyi klonlayın
git clone https://github.com/nurhatipoglu/Rest-API-Golang.git

cd Rest-API-Golang

### Docker kapsayıcısında bir PostgreSQL veritabanı sunucusu başlatın
make db-start

### Bazı test verileriyle veritabanını oluşturun
make testdata

### API sunucusunu çalıştırın
make run

"http://127.0.0.1:8080" adresinde çalışan bir API sunucunuz var.Aşağıdaki uç noktaları sağlar:

* `GET /healthcheck`: durum denetimi amacıyla sağlanan bir sağlık denetimi hizmeti (bir sunucu kümesini uygularken gereklidir)
* `POST /v1/login`: bir kullanıcının kimliğini doğrular ve bir JWT oluşturur
* `GET /v1/albums`: albümlerin sayfalandırılmış bir listesini döndürür
* `GET /v1/albums/:id`: bir albümün ayrıntılı bilgilerini döndürür
* `POST /v1/albums`: yeni bir albüm oluşturur
* `PUT /v1/albums/:id`: mevcut bir albümü günceller
* `DELETE /v1/albums/:id`: bir albümü siler