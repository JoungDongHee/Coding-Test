# (Level 0) 조건 문자열 - 181934 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181934) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

문자열에 따라 다음과 같이 두 수의 크기를 비교하려고 합니다.

* 두 수가 `n`과 `m`이라면

* ">", "=" : `n` >= `m`
* "<", "=" : `n` <= `m`
* ">", "!" : `n` > `m`
* "<", "!" : `n` < `m`

두 문자열 `ineq`와 `eq`가 주어집니다. `ineq`는 "<"와 ">"중 하나고, `eq`는 "="와 "!"중 하나입니다. 그리고 두 정수 `n`과 `m`이 주어질 때, `n`과 `m`이 `ineq`와 `eq`의 조건에 맞으면 1을 아니면 0을 return하도록 solution 함수를 완성해주세요.

##### 제한 사항

* 1 ≤ `n`, `m` ≤ 100

##### 입출력 예

| ineq | eq | n | m | result |
| --- | --- | --- | --- | --- |
| "<" | "=" | 20 | 50 | 1 |
| ">" | "!" | 41 | 78 | 0 |

##### 입출력 예 설명

입출력 예 #1

* 20 <= 50은 참이기 때문에 1을 return합니다.

입출력 예 #2

* 41 > 78은 거짓이기 때문에 0을 return합니다.

※ 2023.05.31 테스트 케이스가 수정되었습니다. 기존에 제출한 코드가 통과하지 못할 수도 있습니다.

### 제출 코드

```java
class Solution {
    public int solution(String ineq, String eq, int n, int m) {
        
        if(ineq.equals(">")){
            if(eq.equals("=")){
                return n >= m ? 1:0;
            }
            return n>m ? 1:0;
        }else {
            if(eq.equals("=")){
                return n <= m ? 1:0;
            }
            return n<m ? 1:0;
        }
    }
}
```

## 제출 일자

2026년 06월 18일 23:04:03

## 성능 요약

메모리: 74.3 MB, 시간: 0.02 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges