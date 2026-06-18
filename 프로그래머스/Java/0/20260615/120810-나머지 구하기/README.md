# (Level 0) 나머지 구하기 - 120810 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/120810) 

## 구분

코딩테스트 연습 > 코딩테스트 입문

## 문제 설명

정수 `num1`, `num2`가 매개변수로 주어질 때, `num1`를 `num2`로 나눈 나머지를 return 하도록 solution 함수를 완성해주세요.

#### 제한사항

* 0 < `num1` ≤ 100
* 0 < `num2` ≤ 100

#### 입출력 예

| num1 | num2 | result |
| --- | --- | --- |
| 3 | 2 | 1 |
| 10 | 5 | 0 |

#### 입출력 예 설명

입출력 예 #1

* `num1`이 3, `num2`가 2이므로 3을 2로 나눈 나머지 1을 return 합니다.

입출력 예 #2

* `num1`이 10, `num2`가 5이므로 10을 5로 나눈 나머지 0을 return 합니다.

### 제출 코드

```java
class Solution {
    public int solution(int num1, int num2) {
        boolean result = validCheck(num1,num2);
        if(result){
            return num1%num2;
        }
        return 0;
    }
    
    private boolean validCheck(int num1 , int num2){
        if(num1 > 0 && num1 <=100 && num2 > 0 && num2 <=100){
            return true;
        }
        return false;
    }
}
```

## 제출 일자

2026년 06월 15일 23:00:27

## 성능 요약

메모리: 75 MB, 시간: 0.02 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges