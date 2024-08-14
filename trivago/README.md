# trivago
---
- site : https://www.trivago.co.kr/

## 크롤링 방법

- Language : Python
- Library : selenium
- url : https://www.trivago.co.kr/ko-KR/srl?search=200-{코드};dr-{시작날짜}-{종료날짜}-s;rc-{객실수}-{성인수}-{어린이나이*어린이수}

### 예시
- 지역날짜 : 서울
- 시작날짜 : 20240821
- 종료날짜 : 20240824
- 객실 수 : 2
- 성인 수 : 3
- 어린이 수 : 2명, 나이 7, 8
>  https://www.trivago.co.kr/ko-KR/srl?search=200-81322;dr-20240821-20240824-s;rc-2-3-7-8


### 실행 방법
```python
cd trivago

crawling.py 
```

### 실행결과
```
서울 호텔 리스트
호텔: 보코서울강남
가격: ₩1,216,346
---
호텔: The Stay Classic Hotel Myeongdong
가격: ₩388,147
---
호텔: ENA Suite Hotel Namdaemun
가격: ₩517,870
---
호텔: 롯데시티호텔 마포
가격: ₩432,667
---
호텔: Le Collective Seoul Seocho
가격: ₩409,682
---
호텔: 호텔 쿠레타케소 서울 인사동
가격: ₩318,166
---
호텔: 보코서울강남
가격: ₩696,630
---
호텔: Friendly Dh Naissance Hotel By Mindrum Group
가격: ₩231,199
---
호텔: Hotel Atrium Jongno
가격: ₩447,169
---
호텔: 에이큐브 호텔
가격: ₩224,375
---
호텔: AC Hotel by Marriott Seoul Gangnam
가격: ₩701,250
---
호텔: 현대 레지던스 서울
가격: ₩310,256
---

```


현재 첫 페이지만 가져오는 방식을 취했고, api로 가져오는 방법을 공부해볼 예정