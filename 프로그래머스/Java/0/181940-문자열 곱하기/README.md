# (Level 0) 문자열 곱하기 - 181940 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181940) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

문자열 `my_string`과 정수 `k`가 주어질 때, `my_string`을 `k`번 반복한 문자열을 return 하는 solution 함수를 작성해 주세요.

##### 제한사항

* 1 ≤ `my_string`의 길이 ≤ 100
* `my_string`은 영소문자로만 이루어져 있습니다.
* 1 ≤ `k` ≤ 100

##### 입출력 예

| my_string | k | result |
| --- | --- | --- |
| "string" | 3 | "stringstringstring" |
| "love" | 10 | "lovelovelovelovelovelovelovelovelovelove" |

##### 입출력 예 설명

입출력 예 #1

* 예제 1번의 `my_string`은 "string"이고 이를 3번 반복한 문자열은 "stringstringstring"이므로 이를 return 합니다.

입출력 예 #2

* 예제 2번의 `my_string`은 "love"이고 이를 10번 반복한 문자열은 "lovelovelovelovelovelovelovelovelovelove"이므로 이를 return 합니다.

### 제출 코드

```java
class Solution {
    public String solution(String my_string, int k) {
        return my_string.repeat(k);
    }
}
```

## 제출 일자

2026년 06월 18일 00:15:08

## 성능 요약

메모리: 73.4 MB, 시간: 0.05 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges