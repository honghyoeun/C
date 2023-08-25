**Q7 포인터 + 반복문 (정보처리기사 21년 2회)**
````
int main(){

  int ary[3];
  int s = 0;
    *(ary+0)=1;
       ary[1] = *(ary+0)+2;
       ary[2] = *ary+3;
          for(int i=0; i<3; i++){
   s=s+ary[i]
}

print("%d",s);

}
````
**Q8 (정보처리기사 21년 2회)**
````
int main(){
   int res;
   res = mp(2,10);
   printf("%d",res);
   return 0;
}

int mp(int base, int exp) {
   int res = 1;
   for(int i=0; i < exp; i++){
      res = res * base;
   }
   
   return res;
}
````
**Q9 (정보처리기사 21년 3회)**
````
#include <stdio.h>
 
int main(){
   int *arr[3];
   int a = 12, b = 24, c = 36;
     arr[0] = &a;
     arr[1] = &b;
     arr[2] = &c;
 
printf("%d\n", *arr[1] + **arr + 1);
 
}
````

**Q10 (정보처리기사 21년 3회)**
````
#include <stdio.h>
 
struct jsu {
  char name[12];
  int os, db, hab, hhab;
};
 
int main(){
struct jsu st[3] = {{"데이터1", 95, 88}, 
                    {"데이터2", 84, 91}, 
                    {"데이터3", 86, 75}};
struct jsu* p;
 
p = &st[0];
 
(p + 1)->hab = (p + 1)->os + (p + 2)->db;
(p + 1)->hhab = (p+1)->hab + p->os + p->db;
 
printf("%d\n", (p+1)->hab + (p+1)->hhab);
}
````

**Q7-Q8 손코딩**
![image](https://github.com/honghyoeun/C/assets/77725041/2ad0a5d6-a2ba-43f7-b56e-496a755e5586)

**Q9-Q10 손코딩**
![image](https://github.com/honghyoeun/C/assets/77725041/afe14c4e-1b4e-4063-b9d6-d5758d86a672)
