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
### 반복문
* 다중 반복문에서 continue, break 를 loop를 설정하면 설정된 반복문을 기준으로 빠져나옴    
      
      loop@for(i in 1 .. 10){
        for(j in 1..10){
        if (i == 1 && j == 2)break@loop
        println("i: $i, j: $j")}
      }
### 클래스
* 클래스는 인스턴스를 만드는 틀
* 인스턴스는 클래스를 이용해서 만들어 내는 서로 다른 속성의 객체를 지칭하는 용어

      class Person (var name:String, val birthYear:Int) {
            fun introduce(){
                  println("안녕하세요. ${birthYear}년생 ${name}입니다.")
            }
      }
* init함수 - 인스턴스 생성시 호출
      
      class Person (var name:String, val birthYear:Int) {
           init{
            println("${this.birthYear}년생 ${this.name}님이 생성되었습니다.")
            }
      }
#### 생성자
* 기본 생성자
      
      (var name:String, val birthYear:Int)
* 보조 생성자
      
      constructor(name:String) :this(name,1997) {
        println("보조 생성자가 사용되었습니다.")
      }
### 상속
1. 이미 존재하는 클래스를 확장하여 새로운 속성이나 함수를 추가한 클래스를 만들어야 할 때
2. 클래스들의 공통점을 모아 코드관리를 편하게 할 때
##### 주의사항
* 수퍼 클래스에 존재하는 속성과 같은 이름의 속성을 가질 수 없음
* 서브 클래스가 생성될 때 반드시 수퍼클래스의 생성자까지 호출되어야 함
