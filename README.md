# JAVA_For  

## ✅for문은 반복문 중 하나로, 정해진 횟수만큼 어떤 작업을 반복하고 싶을 때 사용  

형식  
```
for (초기식; 조건식; 증감식) {
    // 반복해서 실행할 코드
}
```
짝수만 출력  
```
for (int i = 2; i <= 10; i += 2) {
    System.out.println(i);
}
```


1~10까지의 합 구하기  
```
int sum = 0;
for (int i = 1; i <= 10; i++) {
    sum += i;
}
System.out.println("합계: " + sum);
```


## ✅ while문은 조건이 참(true)인 동안 계속 반복되는 반복문.  

형식
```
while (조건식) {
    // 조건이 true일 때 반복 실행할 코드
}
```
```
int i = 1;
while (i <= 5) {
    System.out.println(i);
    i++;
}
```


for문은 정해준 횟수가 있을때 사용한다.  
while문은 횟수를 모를 때 , 조건만 있을 때 적합하다.  


## ✅do-while문은 조건에 상관없이 코드 블록을 최소 1번은 실행하는 반복문.  

```
do {
    // 반복할 코드
} while (조건식);
```

While문은 반복 전에 검사하여 조건이 false면 한 번도 실행 안 됨.  
Do While문은 반복 후에 검사하여 조건이 false여도 최소 한 번 실행됨.  
