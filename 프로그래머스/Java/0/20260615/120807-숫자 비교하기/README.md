# (Level 0) 숫자 비교하기 - 120807 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/120807) 

## 구분

코딩테스트 연습 > 코딩테스트 입문

## 문제 설명

정수 `num1`과 `num2`가 매개변수로 주어집니다. 두 수가 같으면 1 다르면 -1을 retrun하도록 solution 함수를 완성해주세요.

##### 제한사항

* 0 ≤ `num1` ≤ 10,000
* 0 ≤ `num2` ≤ 10,000

##### 입출력 예

| num1 | num2 | result |
| --- | --- | --- |
| 2 | 3 | -1 |
| 11 | 11 | 1 |
| 7 | 99 | -1 |

##### 입출력 예 설명

입출력 예 설명 #1

* `num1`이 2이고 `num2`가 3이므로 다릅니다. 따라서 -1을 return합니다.

입출력 예 설명 #2

* `num1`이 11이고 `num2`가 11이므로 같습니다. 따라서 1을 return합니다.

입출력 예 설명 #3

* `num1`이 7이고 `num2`가 99이므로 다릅니다. 따라서 -1을 return합니다.

### 제출 코드

```java
class Solution {
    public int solution(int num1, int num2) {
        if(num1 >= 0 && num1<= 10000 && num2 >= 0 && num2<= 10000){
            if(num1==num2){
                return 1;
            }
        }
        
        return -1;
    }
}
```

## 제출 일자

2026년 06월 15일 23:00:10

## 성능 요약

메모리: 75.2 MB, 시간: 0.02 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges