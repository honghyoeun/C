**Q1**
````
// char 형 배열 ch를 선언하고 크기가 5인 배열
char ch[5];

// char 형 배열 str을 선언하고 문자열 "abcde"로 초기화, 문자열의 크기에는 널 종료 문자('\0')가 포함
char str[] = "abcde";

// int 형 배열 num을 선언하고 요소가 1, 2, 3, 4, 5로 초기화
int num[] = {1, 2, 3, 4, 5};

// sizeof 연산자를 사용하여 각 배열의 크기를 출력
// sizeof 연산자는 주어진 변수 또는 데이터 형식의 크기를 바이트 단위로 반환

// sizeof(ch)는 char 형 배열 ch의 크기를 바이트 단위로 반환 
printf("%d, ", sizeof(ch));

// sizeof(str)는 char 형 배열 str의 크기를 바이트 단위로 반환
// "abcde" 문자열의 길이는 5이지만 널 종료 문자('\0')가 추가되어 6
printf("%d, ", sizeof(str));

// sizeof(num)은 int 형 배열 num의 크기를 바이트 단위로 반환
// 배열 num에는 5개의 int 요소가 있고, int는 보통 4바이트이므로 sizeof(num)은 20
// sizeof(int)는 int 데이터 형식의 크기를 반환
printf("%d, ", sizeof(num) / sizeof(int));
//. int 배열 num은 5개의 int 요소를 가지고 있고, 각 int는 일반적으로 4바이트, 따라서 sizeof(num)은 5 * 4 = 20바이트
//size라는 연산자는 없음
````

## sizeof
- sizeof(char) // sizeof_ char 자료형의 크기_1 바이트
- sizeof(short) // sizeof_ short 자료형의 크기_2 바이트
- sizeof(int) // sizeof_ int 자료형의 크기_4 바이트
- sizeof(long) // sizeof_ long 자료형의 크기_4 바이트
- sizeof(long long) // sizeof_ long long 자료형의 크기_8 바이트


**Q2**
````
#include <stdio.h>

int main() {
    int num[5] = {1, 2, 3}; // 배열 초기화에 세 요소만 사용, 나머지 두 요소는 0으로 초기화
    
    for (int i = 0; i < 5; i++) {
        printf("%d", num[i]);
    }
    
    return 0;
}

// 만약 return 0;이 for 문 안에 있으면 한 번만 실행된다. 출력 결과 : 1

````
````
