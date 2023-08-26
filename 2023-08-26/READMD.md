**Q11 재귀함수 (정보처리기사 22년 1회)**
````
include <stdio.h>
int func(int a) {
  if (a <= 1) return 1;
  return a * func(a - 1);
}
 
int main() {
  int a;
  scanf("%d", &a);
  printf("%d", func(a));
 
}
````

**Q12 역순 출력(정보처리기사 22년 1회)**
````
#include <stdio.h>

int main() {
  int number = 1234;  // 초기 숫자 값
  int div = 10;       // 나눌 값
  int result = 0;     // 결과를 저장할 변수

  while (number > 0) {  // 숫자가 0보다 클 때까지 반복 // > 
    result = result * div;          // 결과에 10을 곱함 // *
    result = result + number % div; // 나머지를 결과에 더함 // +
    number = number / div;          // 숫자를 10으로 나눔 // /
  }

  printf("%d", result);  // 최종 결과 출력
  return 0;
}
````

**Q13 큰 소인수 찾기(정보처리기사 22년 1회)**
````
#include <stdio.h> 

// 주어진 숫자가 소수인지 확인하는 함수
int isPrime(int number) { 
  int i; 
  for (i = 2; i < number; i++) { 
    if (number % i == 0)  // 만약 나누어 떨어진다면
      return 0;           // 소수가 아님을 반환
  } 
  return 1;               // 소수임을 나타내는 반환값
} 
 
int main(void) { 
  int number = 13195;      // 소인수를 찾을 숫자
  int max_div = 0;         // 가장 큰 소인수를 저장할 변수
  int i; 

  for (i = 2; i < number; i++) {
    // i가 소수이고 number가 i로 나누어떨어진다면
    if (isPrime(i) == 1 && number % i == 0) {
      max_div = i;  // i를 가장 큰 소인수로 업데이트
    }
  }

  printf("%d", max_div);  // 가장 큰 소인수 출력
  return 0; 
}

````
