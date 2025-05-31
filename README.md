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
