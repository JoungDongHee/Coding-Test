# (Level 0) 두 수의 곱 구하기 - 120804 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/120804) 

## 구분

코딩테스트 연습 > 코딩테스트 입문

## 문제 설명

정수 `num1`, `num2`가 매개변수 주어집니다. `num1`과 `num2`를 곱한 값을 return 하도록 solution 함수를 완성해주세요.

#### 제한사항

* 0 ≤ `num1` ≤ 100
* 0 ≤ `num2` ≤ 100

#### 입출력 예

| num1 | num2 | result |
| --- | --- | --- |
| 3 | 4 | 12 |
| 27 | 19 | 513 |

#### 입출력 예 설명

입출력 예 #1

* `num1`이 3, `num2`가 4이므로 3 * 4 = 12를 return합니다.

입출력 예 #2

* `num1`이 27, `num2`가 19이므로 27 * 19 = 513을 return합니다.

### 제출 코드

```java
class Solution {
    public int solution(int num1, int num2) {
        if(0<=num1 && num1 <= 100 && 0<=num2 && num2 <= 100  ){
             return num1*num2;
        }

       return 0;
    }
}
```

## 제출 일자

2026년 06월 15일 22:59:49

## 성능 요약

메모리: 75.9 MB, 시간: 0.03 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges