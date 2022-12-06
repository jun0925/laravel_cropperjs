# Cropper js

[Cropper.js 사이트로 이동하기](https://fengyuanchen.github.io/cropperjs/)
  
### Cropper 프로젝트 사용하기
목차
- Step 1: Cropper 프로젝트 clone 하기
- Step 2: composer 의존성 폴더 생성하기(vender)
- Step 3: APP_KEY 생성하기
- Step 4: 데이터베이스 설정
- Step 5: 서버 실행 & 확인

# Step 1: Laravel 프로젝트 만들기
아래 명령어로 Laravel Project를 생성합니다.
```bash
git clone https://github.com/jun0925/laravel_cropperjs.git
```

# Step 2: composer 의존성 폴더 생성하기(vender)
```bash
composer install
```

# Step 3: APP_KEY 생성하기
```bash
php artisan key:generate
```


# Step 4: 데이터베이스 설정
데이터 베이스 만들기
```bash
create database cropperjs
```

.evn 파일 생성하기
```bash
copy .env.example .env
```

.env 파일 설정하기
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=cropperjs
DB_USERNAME=username
DB_PASSWORD=password
```

# Step 5: 서버 실행 & 확인
Laravel Project 서버켜기
```bash
php artisan serve
```

이미지 크롭 URL
```bash
http://localhost:8000/crop-image-upload
```
(포트번호는 각 실행환경에서 확인해서 적절하게 넣어줍니다.)