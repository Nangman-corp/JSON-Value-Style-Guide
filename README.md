# JSON Value Style Guide

<aside>
💡 본문은 낭만(Nangman)의 JSON Value에 대한 스타일 가이드 입니다.

</aside>

---
## 목차

---

# 1. 소개(Intro)

---

본 문서는 Nangman의 Value 스타일을 설명합니다.

휴대전화번호, 사업자등록번호 등 사용자마다 표기가 다를 수 있는 값에 대한 가이드입니다.

# 2. 특수기호 정의(Define of special character)

---

특수기호는 [ASCII code](https://xn--ko-jnk.wikipedia.org/wiki/ASCII)에 정의된 특수기호 만을 사용합니다.
    

하이픈, 붙임표(Hyphen) : ASCII code 십진수 45에 해당하는 - 을 의미

컴마, 쉼표(comma) : ASCII code 십진수 44에 해당하는 , 을 의미

닷, 마침표(dot) : ASCII code 십진수 46에 해당하는 . 을 의미

# 3. 수치형 데이터(numerical data)

---

수치형(numerical)은 대게 하이픈(-)으로 표기하는 값을 의미합니다.

- 전화번호
- 주민등록번호
- 사업자등록번호

### Server ↔ Client

- 서버와 클라이언트 통신에서는 하이픈(-) 없이 값을 주고 받습니다.
- 반드시 String 값으로 주고 받습니다.

```json
//example
{
	"phoneNumber" : "01091462043"
}
```

# 4. 날짜형 데이터(Date data)

---

날짜형(numerical) 데이터의 경우 전체 날짜와 시간을 포함한 경우를 의미합니다.

ISO 8601 표준에서 UTC 기준시 표기는 한국을 기준으로 하며 생략하여 표기합니다.

<aside>
💡 yyyy-MM-ddTHH:mm:ss

</aside>

위 포맷 내에서 필요한 데이터만을 추출하여 넘길 수 있습니다.

- yyyy : 4자리 연도(Year)
- MM : 2자리 월(Month)
- dd : 2자리 일(Day)
- HH : 24시각제 2자리 시간(hour)
- mm : 분(minute)
- ss : 초(second)

예시 

(Month, Day, Hour가 필요)

→ 03-30 16

(Hour, Minute이 필요)

→ 16:00

### Server ↔ Client

- 사용하는 언어의 날짜 형식을 사용하되, 날짜 형식이 지원하지 않는 경우 String 값으로 주고 받습니다.
