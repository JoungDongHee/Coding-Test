# (Level 0) 대문자로 바꾸기 - 181877 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181877) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

알파벳으로 이루어진 문자열 `myString`이 주어집니다. 모든 알파벳을 대문자로 변환하여 return 하는 solution 함수를 완성해 주세요.

##### 제한사항

* 1 ≤ `myString`의 길이 ≤ 100,000

* `myString`은 알파벳으로 이루어진 문자열입니다.

##### 입출력 예

| myString | result |
| --- | --- |
| "aBcDeFg" | "ABCDEFG" |
| "AAA" | "AAA" |

### 제출 코드

```java
class Solution {
    public String solution(String myString) {
        return myString.toUpperCase();
    }
}
```

## 제출 일자

2026년 06월 18일 23:18:49

## 성능 요약

메모리: 75.4 MB, 시간: 0.02 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges