# (Level 0) 더 크게 합치기 - 181939 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181939) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

연산 ⊕는 두 정수에 대한 연산으로 두 정수를 붙여서 쓴 값을 반환합니다. 예를 들면 다음과 같습니다.

* 12 ⊕ 3 = 123
* 3 ⊕ 12 = 312

양의 정수 `a`와 `b`가 주어졌을 때, `a` ⊕ `b`와 `b` ⊕ `a` 중 더 큰 값을 return 하는 solution 함수를 완성해 주세요.

단, `a` ⊕ `b`와 `b` ⊕ `a`가 같다면 `a` ⊕ `b`를 return 합니다.

##### 제한사항

* 1 ≤ `a`, `b` < 10,000

##### 입출력 예

| a | b | result |
| --- | --- | --- |
| 9 | 91 | 991 |
| 89 | 8 | 898 |

##### 입출력 예 설명

입출력 예 #1

* `a` ⊕ `b` = 991 이고, `b` ⊕ `a` = 919 입니다. 둘 중 더 큰 값은 991 이므로 991을 return 합니다.

입출력 예 #2

* `a` ⊕ `b` = 898 이고, `b` ⊕ `a` = 889 입니다. 둘 중 더 큰 값은 898 이므로 898을 return 합니다.

### 제출 코드

```java
class Solution {
    public int solution(int a, int b) {
        
        if(a<1 && b >= 10000){
            return 0;
        }
        
        String stringA =  String.valueOf(a);
        String stringB =  String.valueOf(b);
        
        String aPlusB = stringA+stringB;
        String bPlusA = stringB+stringA;
        
        Integer intAB = Integer.parseInt(aPlusB);
        Integer intBA = Integer.parseInt(bPlusA);
        
        if(intAB==intBA){
            return intAB;
        }
        
        int answer = (intAB > intBA) ? intAB : intBA;
        return answer;
    }
}
```

## 제출 일자

2026년 06월 17일 23:51:26

## 성능 요약

메모리: 74.5 MB, 시간: 1.41 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges