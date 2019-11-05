# lease
## setup
git clone https://github.com/dich1/lease.git   
cd lease  
git clone https://github.com/laradock/laradock.git  
cd laradock  
cp env-example .env  
sed -ie 's/APP_CODE_PATH_HOST=..\//APP_CODE_PATH_HOST=..\/src/g' .env  
sed -ie 's/MYSQL_VERSION=latest/MYSQL_VERSION=5.7/g' .env  
rm .enve  
docker-compose up -d workspace nginx mysql  
docker-compose exec workspace bash  
## access
http://127.0.0.1
## how to
https://qiita.com/dich1/items/552b1de430d806fe49ac
## demo
http://lease-1234.herokuapp.com

