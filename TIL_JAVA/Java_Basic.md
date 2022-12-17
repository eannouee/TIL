# Java Basic
> Back to Basic, 계속해서 수정됩니다.
>
## 객체(Object)
속성 + 동작으로 설명할 수 있는 대상을 의미 

## 클래스(Class)
속성이 같은 객체를 대표할 수 있는 대상
- 객체를 정의하는 틀이며 필드(속성)과 메소드(동작)로 구성됨 

## 메소드(Method)
일반적인 프로그램 언어의 함수와 유사, 단 함수는 단순한 기능을 모듈화 한 것이지만 메소드는 객체의 동작(행위)을 정의한다.

## 자바 변수 유형
- 1. 멤버변수
    - 클래스부에 선언된 변수들로 객체의 속성에 해당
   - 인스턴스 변수와 클래스 변수로 구분됨 
- 2. 인스턴스 변수 
    - 클래스가 인스턴스될 때 초기화하는 변수
    - 인스턴스를 통해서만 접근 가능 
- 3. 매개 변수
    - 메소드에 인자로 전달되는 값을 받기 위한 변수
    - 메소드 내에서는 지역변수 처럼 사용
- 4. 지역 변수
    - 메소드 내에서 선언된 변수 
    - 멤버 변수와 동일한 이름을 가질 수 있으며 지역변수가 우선이 됨
- 5. 클래스 변수 
    - static으로 선언된 변수
    - 인스턴스 생성 없이 클래스이름.변수명으로 사용 가능
    - 메인 메소드에서 참조 가능
  
## 인스턴스(Instance)
클래스에서 생성한 객체로 고유한 상태가 존재한다.
- 동일한 클래스에서 생성된 객체라도 필드값과 메소드 내용은 다를 수 있다.

## 생성자 
인스턴스를 생성할 때 초기화 시키는 함수(생성자를 메소드라고 하지 않는다.)
- 생성자의 이름은 해당 클래스와 동일하게 작성한다.
- 파라메터만 다르게 해서 여러 개의 생성자를 만들 수 있다(오버로딩)
- this는 해당 객체 자기 자신의 주소를 가리키는 변수이다.
  - 생성자로 멤버 변수에 값을 넣을 때 사용
  - 생성자에서 다른 생성자를 호출할 때 사용
  - 인스턴스의 주소값을 리턴해주는 메소드를 만들 때 사용 

## 접근 제한자
- private : 같은 클래스 내에서만 사용
- default : 아무것도 정의하지 않았을 때, 같은 클래스와 패키지에서만 사용 가능
- protected : 패키지가 다르면 사용 불가능,단 상속 받았을 경우에는 사용 가능
- public : 어디서든 사용 가능 

## 사용 제한자
- static : 객체 생성 없이 사용하고 싶을 때
- final : 변경이 불가
- abstract : 미완의

## 초기화(Initialization)
자바에서 초기화란 객체를 선언하고 값을 **최초**로 할당하는 것이다.
```Java
int a = 10; //선언과 동시에 초기화
```

```Java
a = 20; //값을 바꾸는 할당(allocation)
```
> 초기화를 하는 이유, 클래스 영역에서 선언할 경우에는 컴파일러가 자동으로 값을 할당 해주나 메소드 영역에서 선언할 경우에는 자동으로 값이 할당되지 않아 에러가 발생하기 때문이다.


