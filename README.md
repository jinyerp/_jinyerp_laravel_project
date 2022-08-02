# JinyERP v1
`지니ERP`는 라라벨 기반의 업무처리 프레임워크 입니다. 다양한 업무 기능들을 모듈화 하여 개별로 설치 사용을 할 수 있습니다.

## 설치 및 실행

- 컴포저를 이용하여 지니ERP 프로젝트를 설치합니다.
```
composer create-project jinyerp/laravel 프로젝트
```

- 지니ERP는 기본적인 UI로 tailwind css를 이용하고 있습니다. nodejs의 npm 명령을 통하여
tailwind css와 리소스를 컴파일 합니다.

```
npm install && npm run build
```

> ui 리소스 컴파일 대신에 개발용 watch 형태로 실행할 수도 있습니다.
```
npm install && npm run dev
```

- php의 내장서버를 통하여 지니ERP를 실행합니다.
```
php artisan serve
```

## 모듈확인 및 설치
지니ERP는 작은 조각의 다양한 모듈로 동작을 합니다. 다음과 같은 명령으로 설치된 모듈을 확인할 수 있습니다.
```
php artisan module:list
```

### 모듈설치
`github` 저장소 또는 `.zip`파일을 이용하여 모듈을 손쉽게 설치 가능합니다.
```
php artisan module:geturl 주소
``` 
