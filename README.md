# carbooking
go mod tidy
go mod edit -replace example.com/greetings=../greetings

mkdir -p db/migration
migrate create -ext sql -dir db/migration -seq user_schema

npm install -g dbdocs
dbdocs login  

https://dbdocs.io/ims.msnegi/car_booking


mv wait-for wait-for.sh
chmod +x wait-for.sh