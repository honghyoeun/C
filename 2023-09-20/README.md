**Q1**
````
#include <stdio.h>

#include <stdio.h>

// 두 정수를 더하는 함수 add 선언
int add(int i, int j) {
    return i + j;
}

// 두 정수를 빼는 함수 sub 선언
int sub(int i, int j) {
    return i - j;
}

void main() {
    int (*pf)(int, int); // 함수 포인터 pf 선언

    pf = add; // 함수 포인터 pf를 add 함수로 초기화
    printf("%d", pf(5, 4)); // pf를 사용하여 add 함수 호출 및 결과 출력

    pf = sub; // 함수 포인터 pf를 sub 함수로 변경
    printf("%d", pf(5, 4)); // pf를 사용하여 sub 함수 호출 및 결과 출력
}

// 출력 결과: 91

````
