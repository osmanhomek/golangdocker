# golangdocker

cd /home/USER/Development/golangdocker
# komutu ile dizine gidilir

docker build -t golangdocker .
#Dizinde bulunan Dockerfile aracılığı ile container build edilir

docker run -it -d -p 8080:8080 --name golangdocker golangdocker:latest
#Son olarak oluşturulan docker 8080 portu ile çalıştırılır

curl -I 192.168.99.100:8080
#Komutu ile go uygulamamızın çalışma durumu kontrol edilir
