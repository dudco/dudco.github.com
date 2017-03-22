---
layout: post
title:  "EDCAN 자바 수업"
date:   2017-03-19 00:00:00 0000
tags: ['자바', '안드로이드', '자바 기본']
author: "dudco"
---

안녕하세요 오늘은 저의 동아리인 EDCAN(에드캔)에서 신입생 대상으로 자바 수업을 진행한 것을 포스팅하려고 합니다.

<span style="font-size: 6px">사실 안드로이드에서 자바는 그렇게 깊게 알 필요 없다생각해서 간단하게 기본만 가르쳐 줍니당...<span>

일단 목차는 다음과 같습니다.<br>
<br>
**<a href="#class">클래스와 인스턴스</a>**<br>
**<a href="#member">클래스 멤버와 인스턴스 멤버</a>**<br>
**<a href="#init">생성자</a>**<br>
**<a href="#overload">오버로딩</a>**<br>
**<a href="#extend">상속</a>**<br>
**<a href="#override">오버라이딩</a>**<br>
**<a href="#abmethod">추상메소드</a>**<br>
**<a href="#inter">인터페이스</a>**
<br><br>

***

#  <span id="class">클래스와 인스턴스</span> #
일단 클래스와 인스턴스에 대해 설명드리자면 다음과 같습니다.


**과자 틀** : 클래스<br>
**과자** : 인스턴스

쉽죠? 그렇게 어려운것이 아닙니당!

실제로 코드에서 확인하면


<strong style="float: left">Main.java</strong><br>
~~~java
class Main(){
    public static void main(String[] args){
        Animal ani = new Animal();
    //  ↑클래스       ↑인스턴스(화)
    }
}
~~~

코드에서는 위와 같다고 볼 수 있습니다.<br>
Animal 클래스가 인스턴스가 되어서 ani라는 변수에 대입되는거죠!
<br><br><br>

***

# <span id="member">클래스 멤버와 인스턴스 멤버</span> #

다음으로는 '클래스 멤버와 인스턴스 멤버' 입니다.

자바에서 '멤버'란 메소드( C언어에서의 함수 )와 변수를 뜻합니다.

다음과 같은 코드가 있다고 가정합니다.

<strong style="float: left">Animal.java</strong><br>
~~~java
class Animal{
    ...

    int age;

    ...
}
~~~


위 Animal이란 클래스는 age라는 멤버를 가지고 있습니다.<br>
이 멤버는 인스턴스마다 각각 다르게 가지고 있는 age라는 멤버입니다.<br>

<strong style="float: left">Main.java</strong><br>
~~~java
class Main{
    public static void main(String[] args){
        Animal a1 = new Animal();
        Animal a2 = new Animal();

        a1.age = 11 // a1의 age는 11
        a2.age = 12 // a2의 age는 12

        System.out.println("a1's age : " + a1.age); // a1's age : 11
        System.out.println("a2's age : " + a2.age); // a2's age : 12
    }
}
~~~
위와 같이 완전히 다른 메모리를 할당받고 다른 변수로 취급이 된다는 얘기 입니다.

즉 현재는 '<span style="color : red;">인스턴스 멤버</span>'입니다.

하지만 만약 모든 동물들의 나이가 같다면? <br>
그렇다면 굳이 각각의 인스턴스마다 멤버를 가지고 있을 필요가 사라집니다.<br>
이럴 때 클래스 멤버로 만들면 됩니다.<br>
바로 그것이 '<span style="color: red">클래스 멤버</span>'입니다.

인스턴스 멤버를 클래스 멤버로 바꾸는 방법은
인스턴스 멤버 앞에 **<span style="color : orange">static</span>** 을 붙이는 것 입니다.

<strong style="float: left">Animal.java</strong><br>
~~~java
class Animal{
    ...

    static int age;

    ...
}
~~~

<strong style="float: left">Main.java</strong><br>
~~~java
class Main{
    public static void main(String[] args){
        Animal a1 = new Animal();
        Animal a2 = new Animal();

        a1.age = 11 // age를 11로

        System.out.println("a1's age : " + a1.age); // a1's age : 11
        System.out.println("a2's age : " + a2.age); // a2's age : 11


        a2.age = 12 // age를 12로

        System.out.println("a1's age : " + a1.age); // a1's age : 12
        System.out.println("a2's age : " + a2.age); // a2's age : 12
    }
}
~~~

<br>
또 클래스 멤버가 되면 굳이 인스턴스에서 멤버에 접근 할 필요가 사라집니다.<br>
따라서 아래와 같이 <span style="color: green">인스턴스 생성없이</span>도 접근이 가능합니다.<br>
<br>

<strong style="float: left">Main.java</strong><br>
~~~java
class Main{
    public static void main(String[] args){
        System.out.println(Animal.age);
    }
}
~~~

<br><br>

***

# <span id="init">생성자</span> #

다음으로는 생성자 입니다.<br>
생성자는 말 그대로 생성할 때 실행되는 메소드입니다.<br>
생성자의 규칙은 '<span style="color: #304ffe">반환형이 없다</span>, <span style="color: #304ffe">클래스 이름과 같다</span>' 입니다.<br>


<strong style="float: left">Animal.java</strong><br>
~~~java
class Animal{
    public Animal(){
        System.out.println("Create Animal!!!");
    }
}
~~~

<strong style="float: left">Main.java</strong><br>
~~~java
class Main{
    public static void main(String[] args){
        Animal ani = new Animal(); // Create Animal!!! (생성자 실행)
    }
}
~~~

<br><br>

***

# <span id="overload">오버로딩</span> #

오버로딩이란 이름이 같은 메소드라도 <span style="color : #00bfa5">인자의 개수</span>나 <span style="color : #00bfa5">인자의 자료형</span>이 다르면 다른 메소드로 인식하는 것 입니다.

<strong style="float: left">Animal.java</strong><br>
~~~java
class Animal{
    public void eat(){
        System.out.println("먹는다!");
    }

    public void eat(String food){
        System.out.println(food + "를 먹는다!");
    }
}
~~~


<strong style="float: left">Main.java</strong><br>
~~~
class Main{
    public static void main(String[] args){
        Animal a = new Animal();
        a.eat(); // 먹는다!
        a.eat("사과"); //사과를 먹는다!
    }
}
~~~

<br><br>

***

# <span id="extend">상속</span> #

OOP(객체지향/Object-Oriented Programming)에서 제일 중요하다고 생각하는 것은<br> '<span style="color: #ffab00">재활용성</span>'이라고 배워왔고, 그렇게 생각합니다.

그리고 그 것을 위해 만들어진 기능이 바로 '<span style="color: red;">상속</span>'입니다.

상속의 기능은 상속받은 자식 클래스는 부모 클래스의 모든 멤버들의 사용이 가능합니다.

<strong style="float: left">Animal.java</strong><br>
~~~java
class Animal{
    public void eat(){
        System.out.println("먹는다!");
    }

    public void sleep(){
        System.out.println("잔다!");
    }
}
~~~

<strong style="float: left">Tiger.java</strong><br>
~~~java
class Tiger extends Animal{
    public void cry(){
        System.out.println("어흥!");
    }
}
~~~

<strong style="float: left">Main.java</strong><br>
~~~java
class Main{
    public static void main(String[] args){
        Tiger t = new Tiger();
        t.eat(); // 먹는다!
        t.sleep(); // 잔다!
//      ↑ 위의 메소드는 부모 클래스로부터 받아온 것
        t.cry(); // 어흥!
    }
}
~~~

<br><br>

***

# <span id="override">오버라이딩</span> #

오버라이딩이란 상속의 기능 중 하나입니다.
바로 부모클래스에 정의되어있는 메소드를 자식 클래스에서 <span style="color: pink">재정의</span> 하는 것 입니다.

(정확한 뜻은 우선순위가 자식 메소드에 먼저 있다는 뜻 입니다.)


<strong style="float: left">Animal.java</strong><br>
~~~java
class Animal{
    public void eat(){
        System.out.println("먹는다!");
    }

    public void sleep(){
        System.out.println("잔다!");
    }
}
~~~

<strong style="float: left">Tiger.java</strong><br>
~~~java
class Tiger extends Animal{
    public void cry(){
        System.out.println("어흥!");
    }

    @override
    public void eat(){
        System.out.println("호랑이가 먹는다!");
    }
}
~~~

<strong style="float: left">Main.java</strong><br>
~~~java
class Main{
    public static void main(String[] args){
        Tiger t = new Tiger();
        t.eat(); // 호랑이가 먹는다!
//      ↑부모클래스의 메소드가 아닌 자식클래스에서 재정의한 메소드가 실행됨
    }
}
~~~

<br><br>

***


# <span id="abmethod">추상 메소드</span> #

추상 메소드란 정의만 되어있고 몸체부분이 없는 메소드입니다.<br>
만약 클래스에 추상메소드가 하나라도 정의되어있다면 그 클래스는 추상클래스가 됩니다.<br>


평범한 메소드를 추상클래스로 만드는 예약어는 <span style="color : red">abstract</span>입니다.<br>

<strong style="float: left">Main.java</strong><br>
~~~java
abstract class Animal{
    ...

    abstract public void eat(); // 상속 한 뒤 반드시 오버라이딩을 해줘야한다.

    ...
}
~~~

<strong style="float: left">Tiger.java</strong><br>
~~~java
class Tiger extends Animal{
    ...

    @override
    public void eat(){ // 오버라이딩 받아 재정의 후 사용.
        System.out.println("먹는다!");
    }

    ...
}
~~~


<strong style="float: left">Main.java</strong><br>
```java
class Tiger extends Animal{
    public static void main(){
        Animal a = new Animal(); // error!! Animal.class가 abstract(추상)클래스여서
        Tiger t = new Tiger();
        t.eat(); // 먹는다!
    }
}
```

<br><br>

***

# <span id="inter">인터페이스</span> #
인터페이스는 추상메소드를 모아 둔 클래스라고 생각하면 됩니다.<br>

<strong style="float: left">AnimalInter.java</strong><br>
~~~
interface AnimalInter{
    ...
    void eat();
    void make();
    void hello();
    ...
}
~~~

<strong style="float: left">Tiger.java</strong><br>
~~~java
class Tiger extends Animal implements AnimalInter{
    ...

    @override
    public void eat(){
        System.out.println("먹는다!");
    }

    @override
    public void make(){
        System.out.println("만든다!");
    }

    @override
    public void hello(){
        System.out.println("안녕!");
    }

    ...
}
~~~

인터페이스는 다중으로 상속받을 수 있습니다.<br>

<br><br>

***

![image](/images/17.03.19-Edcan_Java_Basic/image.jpg)


사실 저도 자바 쪽을 잘하지못해 과연 애들을 가르쳐 줄 수 있을까? 많이 고민을 했었습니다.<br>
그래도 덕분에 더 공부해보면서 저 또한 많이 배울 수 있는 좋은 기회였던 것 같습니다.<br>
감사합니당~
