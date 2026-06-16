# (Level 0) 덧셈식 출력하기 - 181947 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181947) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

두 정수 `a`, `b`가 주어질 때 다음과 같은 형태의 계산식을 출력하는 코드를 작성해 보세요.

```
a + b = c
```

##### 제한사항

* 1 ≤ `a`, `b` ≤ 100

##### 입출력 예

입력 #1

```
4 5
```

출력 #1

```
4 + 5 = 9
```

### 제출 코드

```java
import java.util.Scanner;

public class Solution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        if(a>=1 && b<=100){
            int result = a+b;
            System.out.println(a+" + "+b+" = "+result);
        }
        
    }
    
}
```

## 제출 일자

2026년 06월 16일 23:37:11

## 성능 요약

메모리: 71.9 MB, 시간: 88.22 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges