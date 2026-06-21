# (Level 0) 원소들의 곱과 합 - 181929 

[문제 링크](https://school.programmers.co.kr/learn/courses/30/lessons/181929) 

## 구분

코딩테스트 연습 > 코딩 기초 트레이닝

## 문제 설명

정수가 담긴 리스트 `num_list`가 주어질 때, 모든 원소들의 곱이 모든 원소들의 합의 제곱보다 작으면 1을 크면 0을 return하도록 solution 함수를 완성해주세요.

##### 제한사항

* 2 ≤ `num_list`의 길이 ≤ 10
* 1 ≤ `num_list`의 원소 ≤ 9

##### 입출력 예

| num_list | result |
| --- | --- |
| [3, 4, 5, 2, 1] | 1 |
| [5, 7, 8, 3] | 0 |

##### 입출력 예 설명

입출력 예 #1

* 모든 원소의 곱은 120, 합의 제곱은 225이므로 1을 return합니다.

입출력 예 #2

* 모든 원소의 곱은 840, 합의 제곱은 529이므로 0을 return합니다.

### 제출 코드

```java
import java.util.Arrays;
import java.util.List;
import java.util.stream.Collectors;

class Solution {
    public int solution(int[] num_list) {

        List<Integer> list = Arrays.stream(num_list)
                .boxed()
                .toList();

        int multiply = multiply(list);
        int sum = sumMultiply(list);

        if(multiply < sum){
            return 1;
        }
        return 0;
    }

    private int multiply(List<Integer> list){
        int answer = list.getFirst();
        for(int i=1; i<list.size(); i++){
            answer *= list.get(i);
        }
        return answer;
    }

    private int sumMultiply(List<Integer> list){
        int answer = 0;
        for(int i : list){
            answer =  answer + i;
        }
        System.out.println(answer*answer);
        return answer*answer;
    }
}
```

## 제출 일자

2026년 06월 21일 23:05:56

## 성능 요약

메모리: 79.9 MB, 시간: 2.42 ms

## 채점결과

정확성: 100.0<br/>합계: 100.0 / 100.0

> 출처: 프로그래머스 코딩 테스트 연습, https://school.programmers.co.kr/learn/challenges