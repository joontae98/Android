# Kotlin
### 표기법
 * 파스칼 표기법  - 모든 단어를 대문자로 시작(클래스 이름)
 * 카멜 표기법    - 첫 단어만 소문자로 시작(함수, 변수 이름)
### 변수선언
 * var - 일반적인 경우로 언제든 읽기 쓰기 가능
 * val - 선언시 초기화 가능 중간에 값을 변경할 수 없음
 * 타입추론 가능 - 자료형을 명시하지 않아도 자동으로 타입 명시됨
#### 단일 표현식 함수
      fun add(a: Int, b: Int, c: Int) = a + b + c
#### 조건문 when
      when(a) {
        1 -> println("점수 1입니다.")
        "DiMo" -> println("디모의 코틀린 강좌입니다")
        is Long -> println("Long 타입 입니다.")
        !is String -> println("String 타입이 아닙니다.")
        else -> println("어떤 조건도 만족하지 않습니다.")
    }
