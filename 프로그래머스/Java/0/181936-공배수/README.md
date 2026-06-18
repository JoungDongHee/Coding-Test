# (Level 0) 공배수 - 181936 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181936) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

정수 `number`와 `n`, `m`이 주어집니다. `number`가 `n`의 배수이면서 `m`의 배수이면 1을 아니라면 0을 return하도록 solution 함수를 완성해주세요.

##### 제한사항

* 10 ≤ `number` ≤ 100
* 2 ≤ `n`, `m` < 10

##### 입출력 예

| number | n | m | result |
| --- | --- | --- | --- |
| 60 | 2 | 3 | 1 |
| 55 | 10 | 5 | 0 |

##### 입출력 예 설명

입출력 예 #1

* 60은 2의 배수이면서 3의 배수이기 때문에 1을 return합니다.

입출력 예 #2

* 55는 5의 배수이지만 10의 배수가 아니기 때문에 0을 return합니다.

### 제출 코드

```java
class Solution {
    public int solution(int number, int n, int m) {
        boolean multipleTo2 = (number%n == 0) ? true:false;
        boolean multipleTo3 = (number%m == 0) ? true:false;
        System.out.println(multipleTo2);
        System.out.println(multipleTo3);
        return (multipleTo2&&multipleTo3) ? 1:0;
    }
}
```

## 제출 일자

2026년 06월 18일 23:04:32

## 성능 요약

메모리: 73.6 MB, 시간: 0.17 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges