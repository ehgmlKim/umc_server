# [Bronze V] 시험 성적 - 9498 

[문제 링크](https://www.acmicpc.net/problem/9498) 

### 성능 요약

메모리: 17756 KB, 시간: 216 ms

### 분류

구현

### 문제 설명

<p>시험 점수를 입력받아 90 ~ 100점은 A, 80 ~ 89점은 B, 70 ~ 79점은 C, 60 ~ 69점은 D, 나머지 점수는 F를 출력하는 프로그램을 작성하시오.</p>

### 입력 

 <p>첫째 줄에 시험 점수가 주어진다. 시험 점수는 0보다 크거나 같고, 100보다 작거나 같은 정수이다.</p>

### 출력 

 <p>시험 성적을 출력한다.</p>

### 풀이
```java
import java.util.Scanner;

class Main {
	public static void main(String[] args) {

		Scanner sc = new Scanner(System.in);
		int score = sc.nextInt();
        
		switch(score/10){
		    case 10:
		    case 9:
			System.out.println("A");
			break;
		    case 8:
			System.out.println("B");
			break;
		    case 7:
			System.out.println("C");
			break;
		    case 6:
			System.out.println("D");
			break;
		    default:
			System.out.println("F");
			break;
		}
	}
}   
```
