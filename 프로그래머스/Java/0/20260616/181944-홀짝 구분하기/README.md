# (Level 0) 홀짝 구분하기 - 181944 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181944) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

자연수 `n`이 입력으로 주어졌을 때 만약 `n`이 짝수이면 "`n` is even"을, 홀수이면 "`n` is odd"를 출력하는 코드를 작성해 보세요.

##### 제한사항

* 1 ≤ `n` ≤ 1,000

##### 입출력 예

입력 #1

```
100
```

출력 #1

```
100 is even
```

입력 #2

```
1
```

출력 #2

```
1 is odd
```

※ 2023년 05월 15일 지문이 수정되었습니다.

### 제출 코드

```java
import java.util.Scanner;

public class Solution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        
        if(n>= 1 && n <=1000){
            if(n%2==0){
                System.out.print(n+" is even");
               
            }else{
                 System.out.print(n+" is odd");
            }
         
        }
    }
}
```

## 제출 일자

2026년 06월 16일 23:42:38

## 성능 요약

메모리: 70.4 MB, 시간: 121.33 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges