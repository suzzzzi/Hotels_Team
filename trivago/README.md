# trivago
---
- site : https://www.trivago.co.kr/

## 크롤링 방법

- Language : Python
- Library : selenium
- url : https://www.trivago.co.kr/ko-KR/srl?search=200-{코드};dr-{시작날짜}-{종료날짜}-s;rc-{객실수}-{성인수}-{어린이나이*어린이수}

### 예시
- 지역날짜 : 호치민시
- 시작날짜 : 20240821
- 종료날짜 : 20240824
- 객실 수 : 2
- 성인 수 : 3
- 어린이 수 : 2명, 나이 7, 8
>  https://www.trivago.co.kr/ko-KR/srl?search=200-68089;dr-20240821-20240824-s;rc-2-3-7-8


### 실행 방법
```python
cd trivago

crawling.py 
```