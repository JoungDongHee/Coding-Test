# (Level 0) 문자열 섞기 - 181942 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181942) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

길이가 같은 두 문자열 `str1`과 `str2`가 주어집니다.

두 문자열의 각 문자가 앞에서부터 서로 번갈아가면서 한 번씩 등장하는 문자열을 만들어 return 하는 solution 함수를 완성해 주세요.

##### 제한사항

* 1 ≤ `str1`의 길이 = `str2`의 길이 ≤ 10

* `str1`과 `str2`는 알파벳 소문자로 이루어진 문자열입니다.

##### 입출력 예

| str1 | str2 | result |
| --- | --- | --- |
| "aaaaa" | "bbbbb" | "ababababab" |

### 제출 코드

```java
class Solution {
    public String solution(String str1, String str2) {
        boolean lengthCheck = false;
        if(str1.length()>=1 && str2.length()<=10){
             lengthCheck = str1.length() == str2.length();
        }
        
        if(lengthCheck){
            int strLength = str1.length();
            char[] str1Char = str1.toCharArray();
            char[] str2Char = str2.toCharArray();
            StringBuffer sb = new StringBuffer();
            for(int i=0;i<strLength;i++){
                String str1Value = String.valueOf(str1Char[i]);
                String str2Value = String.valueOf(str2Char[i]);
                sb.append(str1Value+str2Value);
            }
            System.out.println(sb.toString());
            return sb.toString();
        }
        return "";
    }
}
```

## 제출 일자

2026년 06월 17일 00:14:55

## 성능 요약

메모리: 72.5 MB, 시간: 1.74 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges