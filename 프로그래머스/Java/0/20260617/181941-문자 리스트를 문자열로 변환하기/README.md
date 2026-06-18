# (Level 0) 문자 리스트를 문자열로 변환하기 - 181941 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181941) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

문자들이 담겨있는 배열 `arr`가 주어집니다. `arr`의 원소들을 순서대로 이어 붙인 문자열을 return 하는 solution함수를 작성해 주세요.

##### 제한사항

* 1 ≤ `arr`의 길이 ≤ 200

* `arr`의 원소는 전부 알파벳 소문자로 이루어진 길이가 1인 문자열입니다.

##### 입출력 예

| arr | result |
| --- | --- |
| ["a","b","c"] | "abc" |

### 제출 코드

```java
class Solution {
    public String solution(String[] arr) {
        StringBuilder sb = new StringBuilder();
        if(arr.length>=1 && arr.length<=200){
            for(String value : arr){
                sb.append(value);
            }
            return sb.toString();
        }
        return "";
    }
}
```

## 제출 일자

2026년 06월 17일 23:36:42

## 성능 요약

메모리: 73.4 MB, 시간: 0.03 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges