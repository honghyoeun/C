**Q4**
````
#include <stdio.h>

int fn(char* a) {
    int i = 0;
    for (i = 0; a[i] != '\0'; i++);
    return i;
}

int main() { // main 함수의 반환 타입을 int로 수정
    char a[10] = "Hello";
    printf("%d", fn(a)); // 5출력
    return 0; // main 함수의 반환 값으로 0을 반환 
}

````

**Q5**
````
#include <stdio.h>

// 함수 선언
int f(int i);

int main() { // main 함수의 반환 타입을 int로 수정
    // 함수 f를 호출하고 결과를 출력
    printf("%d %d %d", f(1), f(5), f(-2));
    return 0; // main 함수의 반환 값으로 0을 반환
}

int f(int i) {
    if (i <= 2)
        return 1;
    else
        return f(i - 1) + f(i - 2);
}

````
