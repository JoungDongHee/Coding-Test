# (Level 0) n의 배수 - 181937 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181937) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

정수 `num`과 `n`이 매개 변수로 주어질 때, `num`이 `n`의 배수이면 1을 return `n`의 배수가 아니라면 0을 return하도록 solution 함수를 완성해주세요.

##### 제한사항

* 2 ≤ `num` ≤ 100
* 2 ≤ `n` ≤ 9

##### 입출력 예

| num | n | result |
| --- | --- | --- |
| 98 | 2 | 1 |
| 34 | 3 | 0 |

##### 입출력 예 설명

입출력 예 #1

* 98은 2의 배수이므로 1을 return합니다.

입출력 예 #2

* 32는 3의 배수가 아니므로 0을 return합니다.

### 제출 코드

```java
class Solution {
    public int solution(int num, int n) {
        return (num%n==0) ? 1:0;
    }
}
```

## 제출 일자

2026년 06월 18일 23:04:43

## 성능 요약

메모리: 79.1 MB, 시간: 0.03 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges