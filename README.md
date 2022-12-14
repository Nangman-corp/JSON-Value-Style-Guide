# JSON Value Style Guide

<aside>
π‘ λ³Έλ¬Έμ λ­λ§(Nangman)μ JSON Valueμ λν μ€νμΌ κ°μ΄λ μλλ€.

</aside>


## λͺ©μ°¨
---
### [1. μκ°(Intro)](https://github.com/Nangman-corp/JSON-Value-Style-Guide/blob/main/README.md#1-%EC%86%8C%EA%B0%9Cintro-1)
### [2. νΉμκΈ°νΈ μ μ(Define of special character)](https://github.com/Nangman-corp/JSON-Value-Style-Guide/blob/main/README.md#2-%ED%8A%B9%EC%88%98%EA%B8%B0%ED%98%B8-%EC%A0%95%EC%9D%98define-of-special-character-1)
### [3. μμΉν λ°μ΄ν°(numerical data)](https://github.com/Nangman-corp/JSON-Value-Style-Guide/blob/main/README.md#3-%EC%88%98%EC%B9%98%ED%98%95-%EB%8D%B0%EC%9D%B4%ED%84%B0numerical-data-1)
### [4. λ μ§ν λ°μ΄ν°(Date data)](https://github.com/Nangman-corp/JSON-Value-Style-Guide/blob/main/README.md#4-%EB%82%A0%EC%A7%9C%ED%98%95-%EB%8D%B0%EC%9D%B4%ED%84%B0date-data-1)

---

# 1. μκ°(Intro)

---

λ³Έ λ¬Έμλ Nangmanμ Value μ€νμΌμ μ€λͺν©λλ€.

ν΄λμ νλ²νΈ, μ¬μμλ±λ‘λ²νΈ λ± μ¬μ©μλ§λ€ νκΈ°κ° λ€λ₯Ό μ μλ κ°μ λν κ°μ΄λμλλ€.

# 2. νΉμκΈ°νΈ μ μ(Define of special character)

---

νΉμκΈ°νΈλ [ASCII code](https://xn--ko-jnk.wikipedia.org/wiki/ASCII)μ μ μλ νΉμκΈ°νΈ λ§μ μ¬μ©ν©λλ€.
    

νμ΄ν, λΆμν(Hyphen) : ASCII code μ­μ§μ 45μ ν΄λΉνλ - μ μλ―Έ

μ»΄λ§, μΌν(comma) : ASCII code μ­μ§μ 44μ ν΄λΉνλ , μ μλ―Έ

λ·, λ§μΉ¨ν(dot) : ASCII code μ­μ§μ 46μ ν΄λΉνλ . μ μλ―Έ

# 3. μμΉν λ°μ΄ν°(numerical data)

---

μμΉν(numerical)μ λκ² νμ΄ν(-)μΌλ‘ νκΈ°νλ κ°μ μλ―Έν©λλ€.

- μ νλ²νΈ
- μ£Όλ―Όλ±λ‘λ²νΈ
- μ¬μμλ±λ‘λ²νΈ

### Server β Client

- μλ²μ ν΄λΌμ΄μΈνΈ ν΅μ μμλ νμ΄ν(-) μμ΄ κ°μ μ£Όκ³  λ°μ΅λλ€.
- λ°λμ String κ°μΌλ‘ μ£Όκ³  λ°μ΅λλ€.

```json
//example
{
	"phoneNumber" : "01091462043"
}
```

# 4. λ μ§ν λ°μ΄ν°(Date data)

---

λ μ§ν(numerical) λ°μ΄ν°μ κ²½μ° μ μ²΄ λ μ§μ μκ°μ ν¬ν¨ν κ²½μ°λ₯Ό μλ―Έν©λλ€.

ISO 8601 νμ€μμ UTC κΈ°μ€μ νκΈ°λ νκ΅­μ κΈ°μ€μΌλ‘ νλ©° μλ΅νμ¬ νκΈ°ν©λλ€.

<aside>
π‘ yyyy-MM-ddTHH:mm:ss

</aside>

μ ν¬λ§· λ΄μμ νμν λ°μ΄ν°λ§μ μΆμΆνμ¬ λκΈΈ μ μμ΅λλ€.

- yyyy : 4μλ¦¬ μ°λ(Year)
- MM : 2μλ¦¬ μ(Month)
- dd : 2μλ¦¬ μΌ(Day)
- HH : 24μκ°μ  2μλ¦¬ μκ°(hour)
- mm : λΆ(minute)
- ss : μ΄(second)

μμ 

(Month, Day, Hourκ° νμ)

β 03-30 16

(Hour, Minuteμ΄ νμ)

β 16:00

### Server β Client

- μ¬μ©νλ μΈμ΄μ λ μ§ νμμ μ¬μ©νλ, λ μ§ νμμ΄ μ§μνμ§ μλ κ²½μ° String κ°μΌλ‘ μ£Όκ³  λ°μ΅λλ€.

---

### Contributors
---
- [Contributors](https://github.com/Nangman-corp/JSON-Value-Style-Guide/graphs/contributors)
