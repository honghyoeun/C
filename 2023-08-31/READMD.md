**Q18**
````
#include <stdio.h>  // 표준 입력과 출력을 위한 라이브러리를 포함

// 주어진 숫자가 소수인지 판별하는 함수
int Q18(int num) {
    int i;
    for(i = 2; i < num; i++) {  // 2부터 num보다 작은 수까지 반복
        if(num % i == 0)  // num을 i로 나눴을 때 나머지가 0이면 나누어 떨어지는 수
            return 0;  // 나누어 떨어지는 수이므로 소수가 아님
    }
    return 1;  // 나누어 떨어지는 수가 없으므로 소수
}

// 프로그램 시작점
void main() {
    int num = 10, cnt = 0, i;

    for(i = 2; i < num; i++) {  // 2부터 num보다 작은 수까지 반복
        cnt += Q18(i);  // Q18 함수를 호출하여 소수인지 검사하고, 소수일 경우 cnt를 증가
    }

    printf("%d\n", cnt);  // 소수의 개수를 출력
}

````

**Q19**
````
#include<stdio.h>
#include<stdlib.h>
#include<time.h>

  void main(0 {
   int has[6] = {0,};
   int n, i = 0;
     srand(time(NULL));
do{
 i++;
 n = rand()%6 + 1;
 hist[___1___] +=1;
}while(i<10);
}
 for(i=0; i<6; i++)
 printf("h[%d] = %d\n", i, ___2___)
````

**Q20**
````
#include <stdio.h>
void main() 
 int num[10];
 int min = 9999;
 int i;
   for(i=0; i<10; i++) {
 scanf("%d", &num[i]); 
}
   for(i=0; i<10; i++) {
 if(min > __________) {
 min = num[i];
 ]
}
 print("%d", min);
}
````
