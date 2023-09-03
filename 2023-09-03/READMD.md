**Q1**
````
#include <stdio.h>      // 표준 입력과 출력을 위한 헤더 파일 포함
#include <string.h>     // 문자열 관련 함수를 사용하기 위한 헤더 파일 포함

int main(int argc, char *argv[]) {
    // 문자열을 저장할 배열 선언 및 초기화
    char str1[20] = "KOREA";
    char str2[20] = "LOVE";
    
    // 포인터 변수 선언 및 초기화
    char* p1 = NULL;
    char* p2 = NULL;
    p1 = str1;   // p1이 str1을 가리키도록 설정
    p2 = str2;   // p2가 str2를 가리키도록 설정
    
    // 문자열 배열의 특정 인덱스에 다른 문자 할당
    str1[1] = p2[2];   // str1 배열의 두 번째 요소에 str2 배열의 세 번째 요소인 'V'를 할당
    str2[3] = p1[4];   // str2 배열의 네 번째 요소에 str1 배열의 다섯 번째 요소인 'A'를 할당
    
    // 두 문자열을 이어붙이기
    strcat(str1, str2);   // str1 뒤에 str2를 이어붙임
    
    // 포인터를 사용하여 결과 출력
    printf("%c", *(p1 + 2));   // p1을 이용하여 str1의 세 번째 문자 출력 ('R')

    return 0;   // 프로그램 종료
}

````

**Q2**
````
#include <stdio.h>   // 표준 입력과 출력을 위한 헤더 파일 포함

int main(int argc, char *argv[]) {
    // 2x3 배열 선언 및 초기화
    int arr[2][3] = {{1, 2, 3}, {4, 5, 6}};
    
    // 포인터 변수 선언 및 초기화
    int (*p)[3] = NULL;
    p = arr;  // p가 arr을 가리키도록 설정

    // 첫 번째 출력: arr[0][1] + arr[1][2]
    printf("%d", *(p[0] + 1) + *(p[1] + 2));

    // 두 번째 출력: arr[1][0] + arr[1][1]
    printf("%d", *(*(p + 1) + 0) + *(*(p + 1) + 1));

    return 0;  // 프로그램 종료
}

````

**Q3**
````
#include <stdio.h>

int main(int argc, char *argv[]) {
    // 변수 선언
    int n1 = 1, n2 = 2, n3 = 4; // n1, n2, n3를 초기화

    int r1, r2, r3;

    // 논리식 평가 및 결과 저장
    r1 = (n2 <= 2) || (n3 > 3); // n2가 2 이하이거나 n3가 3 초과인 경우 r1은 참(1), 아니면 거짓(0)
    r2 = !n3; // n3가 0이 아니면 r2는 거짓(0), 0이면 참(1)
    r3 = (n1 > 1) && (n2 < 3); // n1이 1 초과이고 n2가 3 미만인 경우 r3는 참(1), 아니면 거짓(0)

    // 결과 출력
    printf("%d", r3 - r2 + r1); // r3 - r2 + r1의 결과를 출력

    return 0;
}

````

