# (Level 0) 두 수의 연산값 비교하기 - 181938 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181938) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

연산 ⊕는 두 정수에 대한 연산으로 두 정수를 붙여서 쓴 값을 반환합니다. 예를 들면 다음과 같습니다.

* 12 ⊕ 3 = 123
* 3 ⊕ 12 = 312

양의 정수 `a`와 `b`가 주어졌을 때, `a` ⊕ `b`와 `2 * a * b` 중 더 큰 값을 return하는 solution 함수를 완성해 주세요.

단, `a` ⊕ `b`와 `2 * a * b`가 같으면  `a` ⊕ `b`를 return 합니다.

##### 제한사항

* 1 ≤ `a`, `b` < 10,000

##### 입출력 예

| a | b | result |
| --- | --- | --- |
| 2 | 91 | 364 |
| 91 | 2 | 912 |

##### 입출력 예 설명

입출력 예 #1

* `a` ⊕ `b` = 291 이고, `2 * a * b` = 364 입니다. 둘 중 더 큰 값은 364 이므로 364를 return 합니다.

입출력 예 #2

* `a` ⊕ `b` = 912 이고, `2 * a * b` = 364 입니다. 둘 중 더 큰 값은 912 이므로 912를 return 합니다.

※ 2023년 04월 27일 입출력 예 설명이 수정되었습니다.

### 제출 코드

```java
class Solution {
    public int solution(int a, int b) {
        int plusResult = plus(a,b);
        int multiResilt = multiplication(a,b);
        
        System.out.println(plusResult);
        System.out.println(multiResilt);
        
        if(plusResult == multiResilt){
            return plusResult;
        }
        
        return (plusResult>multiResilt) ? plusResult:multiResilt;
    }
    
    
    private int plus(int a,int b){
        String aPlusB =  String.valueOf(a)+String.valueOf(b);
        return Integer.parseInt(aPlusB);
    }
    
    private int multiplication(int a , int b){
        return 2*a*b;
    }
}
```

## 제출 일자

2026년 06월 18일 00:00:33

## 성능 요약

메모리: 86.9 MB, 시간: 1.85 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges