# (Level 0) 문자열 겹쳐쓰기 - 181943 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181943) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

문자열 `my_string`, `overwrite_string`과 정수 `s`가 주어집니다. 문자열 `my_string`의 인덱스 `s`부터 `overwrite_string`의 길이만큼을 문자열 `overwrite_string`으로 바꾼 문자열을 return 하는 solution 함수를 작성해 주세요.

##### 제한사항

* `my_string`와 `overwrite_string`은 숫자와 알파벳으로 이루어져 있습니다.
* 1 ≤ `overwrite_string`의 길이 ≤ `my_string`의 길이 ≤ 1,000
* 0 ≤ `s` ≤ `my_string`의 길이 - `overwrite_string`의 길이

##### 입출력 예

| my_string | overwrite_string | s | result |
| --- | --- | --- | --- |
| "He11oWor1d" | "lloWorl" | 2 | "HelloWorld" |
| "Program29b8UYP" | "merS123" | 7 | "ProgrammerS123" |

##### 입출력 예 설명

입출력 예 #1

* 예제 1번의 `my_string`에서 인덱스 2부터 `overwrite_string`의 길이만큼에 해당하는 부분은 "11oWor1"이고 이를 "lloWorl"로 바꾼 "HelloWorld"를 return 합니다.

입출력 예 #2

* 예제 2번의 `my_string`에서 인덱스 7부터 `overwrite_string`의 길이만큼에 해당하는 부분은 "29b8UYP"이고 이를 "merS123"로 바꾼 "ProgrammerS123"를 return 합니다.

### 제출 코드

```java
class Solution {
    public String solution(String my_string, String overwrite_string, int s) {
        // 매개변수 유효 범위 및 제약조건 검사
        if (checkValid(my_string, overwrite_string, s)) {
            // 동기화가 필요 없는 단일 스레드 환경이므로 StringBuilder를 사용하여 성능 최적화
            StringBuilder sb = new StringBuilder(my_string);
            sb.replace(s, s + overwrite_string.length(), overwrite_string);
            return sb.toString();
        }
        
        return "";
    }
    
    // 유효성 검증(Validation check)을 위한 헬퍼 메서드(Helper method)
    private boolean checkValid(String myString, String overwriteString, int s) {
        if (myString == null || overwriteString == null) {
            return false;
        }
        int myLength = myString.length();
        int overLength = overwriteString.length();
        
        return overLength >= 1 && overLength <= myLength && myLength <= 1000
                && s >= 0 && s <= myLength - overLength;
    }
}
```

## 제출 일자

2026년 06월 17일 00:26:19

## 성능 요약

메모리: 77.8 MB, 시간: 0.06 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges