---
title: 자바 직렬화, 그것이 알고싶다.<br/>훑어보기편
date: 2018-01-19 15:54:24
tags: 
- 간다ㅏ
- 라마바
categories:
- tech
- android
author: Jehoon.park

---

자바의 직렬화 기술에 대한 대한 이야기입니다. 간단한 질문과 답변 형태로 자바 직렬화에 대한 간단한 설명과 직접 프로젝트를 진행하면서 겪은 경험에 대해 이야기해보려 합니다. 자바의 직렬화 기술에 대한 대한 이야기입니다. 간단한 질문과 답변 형태로 자바 직렬화에 대한 간단한 설명과 직접 프로젝트
를 진행하면서 겪은 경험에 대해 이야기해보려 합니다.

![석촌호수 러버덕](http://cfile6.uf.tistory.com/image/2426E646543C9B4532C7B0)

## 자바 직렬화가 무엇(what)인가요??
* 자바 직렬화란 자바 시스템 내부에서 사용되는 객체 또는 데이터를 외부의 자바 시스템에서도 사용할 수 있도록 바이트(byte) 형태로 데이터 변환하는 기술과 바이트로 변환된 데이터를 다시 객체로 변환하는 기술(역직렬화)을 아울러서 이야기합니다.
* 시스템적으로 이야기하자면 JVM(Java Virtual Machine 이하 JVM)의 메모리에 상주(힙 또는 스택)되어 있는 객체 데이터를 바이트 형태로 변환하는 기술과 직렬화된 바이트 형태의 데이터를 객체로 변환해서 JVM으로 상주시키는 형태를 같이 이야기합니다.

## 자바 직렬화는 어떻게(how) 사용할 수 있나요?
### 자바 직렬화 조건
자바 기본(primitive) 타입과 java.io.Serializable 인터페이스를 상속받은 객체는 직렬화 할 수 있는 기본 조건을 가집니다.

``` java
package woowahan.blog.exam1;
    /**
    * 직렬 화할 회원 클래스
    */
    public class Member implements Serializable {
        private String name;
        private String email;
        private int age;
    
        public Member(String name, String email, int age) {
            this.name = name;
            this.email = email;
            this.age = age;
        }
    
        // Getter 생략
    
        @Override
        public String toString() {
            return String.format("Member{name='%s', email='%s', age='%s'}", name, email, age);
        }
    }
```