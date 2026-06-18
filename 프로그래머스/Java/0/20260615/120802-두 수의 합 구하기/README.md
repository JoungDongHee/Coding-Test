# (Level 0) 두 수의 합 구하기 - 120802 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/120802) 

## 구분

코딩테스트 연습 > 코딩테스트 입문

## 문제 설명

정수 `num1`과 `num2`가 주어질 때, `num1`과 `num2`의 합을 return하도록 soltuion 함수를 완성해주세요.

##### 제한사항

* -50,000 ≤ `num1` ≤ 50,000
* -50,000 ≤ `num2` ≤ 50,000

#### 입출력 예

| num1 | num2 | result |
| --- | --- | --- |
| 2 | 3 | 5 |
| 100 | 2 | 102 |

##### 입출력 예 설명

입출력 예 #1

* `num1`이 2이고 `num2`가 3이므로 2 + 3 = 5를 return합니다.

입출력 예 #2

* `num1`이 100이고 `num2`가 2이므로 100 + 2 = 102를 return합니다.

### 제출 코드

```java
class Solution {
    public int solution(int num1, int num2) {
        if(checkValid(num1) && checkValid(num2)){
            return num1 + num2;
        }
    
        return 0;
    }
    
    private boolean checkValid(int num){
        if(num >= -50000 && num <= 50000){
            return true;
        }
        return false;
    }
}
```

## 제출 일자

2026년 06월 15일 23:17:23

## 성능 요약

메모리: 74.9 MB, 시간: 0.02 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges