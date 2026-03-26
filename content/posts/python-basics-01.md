---
title: "Python 기초 (1) — 변수와 자료형"
date: 2026-03-26
draft: false
tags: ["Python", "기초", "프로그래밍"]
categories: ["Python"]
description: "Python의 변수 선언 방법과 주요 자료형을 예제와 함께 정리합니다."
---

## 개요

Python은 문법이 간결하고 읽기 쉬운 언어로, 데이터 분석·자동화·AI 분야에서 가장 널리 쓰입니다.
이 시리즈에서는 Python을 처음 배우는 분들을 위해 핵심 개념을 예제 중심으로 설명합니다.

---

## 변수 선언

Python은 타입을 명시하지 않아도 됩니다. 값을 넣으면 자동으로 타입이 결정됩니다.

```python
name = "홍길동"       # 문자열 (str)
age = 30              # 정수 (int)
height = 175.5        # 실수 (float)
is_student = False    # 불리언 (bool)
```

Java와 달리 `String name = "홍길동";` 처럼 타입을 앞에 쓸 필요가 없습니다.

---

## 주요 자료형

### 문자열 (str)

```python
greeting = "안녕하세요"
print(greeting)           # 안녕하세요
print(len(greeting))      # 5 (글자 수)
print(greeting[0])        # 안 (첫 번째 문자)
print(greeting + "!")     # 안녕하세요! (문자열 연결)
```

f-string으로 변수를 문자열에 삽입할 수 있습니다.

```python
name = "홍길동"
age = 30
print(f"{name}의 나이는 {age}세입니다.")
# 홍길동의 나이는 30세입니다.
```

### 리스트 (list)

순서가 있는 값의 묶음. 값을 추가·삭제할 수 있습니다.

```python
fruits = ["사과", "바나나", "딸기"]
print(fruits[0])      # 사과
fruits.append("포도") # 항목 추가
print(len(fruits))    # 4
```

### 딕셔너리 (dict)

키-값 쌍으로 데이터를 저장합니다.

```python
person = {
    "name": "홍길동",
    "age": 30,
    "city": "서울"
}
print(person["name"])   # 홍길동
person["age"] = 31      # 값 수정
```

---

## 타입 확인과 변환

```python
x = "123"
print(type(x))       # <class 'str'>

x = int(x)           # 문자열 → 정수 변환
print(type(x))       # <class 'int'>
print(x + 1)         # 124
```

---

## 핵심 정리

| 자료형 | 예시 | 특징 |
|--------|------|------|
| `str` | `"안녕"` | 문자열, 따옴표로 감쌈 |
| `int` | `42` | 정수 |
| `float` | `3.14` | 실수 |
| `bool` | `True / False` | 참/거짓 |
| `list` | `[1, 2, 3]` | 순서 있는 목록 |
| `dict` | `{"key": "value"}` | 키-값 쌍 |

---

다음 편에서는 **조건문과 반복문** (`if`, `for`, `while`)을 다룹니다.
