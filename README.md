# Python Print Formatting Examples

이 프로젝트는 **파이썬의 다양한 출력 방법**을 예시 코드와 함께 정리한 것입니다.  
`변수 선언`, `print()` 함수 활용, `f-string`, `format()`, `% 포맷팅` 등  
출력 형식을 이해하는 데 도움이 됩니다.

---

## 📌 코드 설명

### 1. 변수 선언
```python
name = "오재언"
age = 227
score = 95.5
```
기본적으로 문자열, 정수, 실수형 변수를 선언합니다.

---

### 2. 기본 출력
```python
print("Hello, Python!")
```
가장 단순한 출력.

---

### 3. 여러 값 출력
```python
print("Name:", name, "Age:", age, "Score:", score)
```
`콤마(,)`로 구분하면 자동으로 공백이 들어갑니다.

---

### 4. f-string (Python 3.6+)
```python
print(f"My name is {name}, I am {age} years old, score: {score}")
```
가장 많이 쓰이는 방법. 중괄호 `{}` 안에서 직접 변수나 계산식을 넣을 수 있습니다.

---

### 5. format() 함수
```python
print("My name is {}, I am {} years old, score: {}".format(name, age, score))
print("My name is {0}, age {1}, score {2}".format(name, age, score))
print("Score with 2 decimals: {:.2f}".format(score))
```
`{}` 안에 순서를 지정하거나, 포맷 옵션을 줄 수 있습니다.

---

### 6. % 포맷팅 (C 스타일)
```python
print("Name: %s, Age: %d, Score: %.1f" % (name, age, score))
```
오래된 방식이지만, 여전히 사용할 수 있습니다.

---

### 7. 여러 줄 출력
```python
print("This is line 1\nThis is line 2")
```
`\n`으로 줄바꿈 처리.

---

### 8. end 옵션
```python
print("Hello", end=" ")
print("world!")
```
줄바꿈 대신 공백으로 끝맺습니다.

---

### 9. sep 옵션
```python
print("2025", "09", "23", sep="-")
```
출력 구분자를 `-`로 변경.

---

### 10. 딕셔너리/리스트 같이 출력
```python
data = {"name": name, "age": age, "score": score}
print("Data", data)
```

---

### 11. f-string 내 계산식/함수 사용
```python
print(f"Next year age: {age + 1}")
print(f"Score (rounded): {round(score)}")
```

---

### 12. 멀티라인 f-string
```python
print(f"""
Student Info:
- Name : {name}
- Age  : {age}
- Score: {score:.2f}
""")
```
여러 줄을 보기 좋게 출력 가능.

---

## 🚀 실행 방법
1. Python 3.6 이상 설치
2. `print_examples.py` (예시 코드 파일) 실행:
   ```bash
   python print_examples.py
   ```

---

## 📝 요약
- `print()`는 다양한 옵션(`sep`, `end`, `\n`)을 제공
- 최신 파이썬에서는 **f-string** 사용을 권장
- `format()`, `% 포맷팅`도 여전히 활용 가능
