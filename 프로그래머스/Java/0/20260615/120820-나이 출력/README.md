# (Level 0) 나이 출력 - 120820 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/120820) 

## 구분

코딩테스트 연습 > 코딩테스트 입문

## 문제 설명

머쓱이는 선생님이 몇 년도에 태어났는지 궁금해졌습니다. 2022년 기준 선생님의 나이 `age`가 주어질 때, 선생님의 출생 연도를 return 하는 solution 함수를 완성해주세요

##### 제한사항

* 0 < age ≤ 120
* 나이는 태어난 연도에 1살이며 매년 1월 1일마다 1살씩 증가합니다.

##### 입출력 예

| age | result |
| --- | --- |
| 40 | 1983 |
| 23 | 2000 |

##### 입출력 예 설명

입출력 예 #1

* 2022년 기준 40살이므로 1983년생입니다.

입출력 예 #2

* 2022년 기준 23살이므로 2000년생입니다.

※ 공지 - 2024년 3월 14일 문제 지문이 보다 명확하게 수정되었습니다.

### 제출 코드

```java
class Solution {
    public int solution(int age) {
        boolean result = checkValid(age);
        int year = 2022;
        if(result){
            return 2022 - age + 1;
        }
        return 0;
    }
    
    private boolean checkValid(int age){
        if(age >0 && age <=120){
            return true;
        }
        return false;
    }
}
```

## 제출 일자

2026년 06월 15일 23:00:55

## 성능 요약

메모리: 73.3 MB, 시간: 0.02 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges