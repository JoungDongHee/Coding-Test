# (Level 0) 문자열 붙여서 출력하기 - 181946 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181946) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

두 개의 문자열 `str1`, `str2`가 공백으로 구분되어 입력으로 주어집니다.

입출력 예와 같이 `str1`과 `str2`을 이어서 출력하는 코드를 작성해 보세요.

##### 제한사항

* 1 ≤ `str1`, `str2`의 길이 ≤ 10

##### 입출력 예

입력 #1

```
apple pen
```

출력 #1

```
applepen
```

입력 #2

```
Hello World!
```

출력 #2

```
HelloWorld!
```

### 제출 코드

```java
import java.util.Scanner;

public class Solution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.next();
        String b = sc.next();
        
        if(a.length()>=1 && b.length() <=10){
            System.out.print(a+b);
        }
    }
}
```

## 제출 일자

2026년 06월 16일 23:38:23

## 성능 요약

메모리: 68 MB, 시간: 91.56 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges