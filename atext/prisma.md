# Prisma

## (01) install

```bash
npm install --save-dev prisma@latest
npm install --save @prisma/client@latest
```

## (02) Prisma 초기화

```bash
# 프리즈마 초기화
npx prisma init
--> prisma 폴더 생성, schema.prisma 생성
```

## (03) schema.prisma 설정

## ➊ generator

```javascript
generator client {
  provider = "pisma-client-js"        # javascript를 이용한 접속
}
```



## ➋ sql

```javascript
datasource db {
  provider = "postgresql"            # 데이터 소스 커넥터
  url      = env("DATABASE_URL")     # .env, 연결 URL
}
```

## ➌ postgresql

```javascript
datasource db {
  provider = "postgresql"            # 데이터 소스 커넥터
  url      = env("DATABASE_URL")     # .env, 연결 URL
}
```





## ➌ ➍ 마

```javascript
generator client {
  provider = "pisma-client-js"
}

datasource db {
  provider = "postgresql"
  url      = env("DATABASE_URL")
}

model Article {
    id Int @id @default(autoincrement())
    title String
    content String
}
```

## ➍ 마이그레이션(database에 테이블 생성)

```bash
npx prisma db push # 모든 테이블 초기
```

===========================================================

➊ ➋ ➌ ➍ ➎ ➏ ➐ ➑ ➒ ➊ ➋ ➌ ➍ ➎ ➏ ➐ ➑ ➒ ➓

(01)(02)(03)(04)(05)(06)(07)(08)(09)(10)(11)(12)(13)(14)(15)(16)(17)(18)(19)(20)

(一)(二)(三)(四)(六)(七)(九)(十)◎

一二三四五六七八九十
