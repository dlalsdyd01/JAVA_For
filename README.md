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

## ✅이중 반복문은 반복문 안에 또 다른 반복문이 있는 구조  

예제) 별 사각형 만들기  
```
public class _08_NestedLoop2 {
    public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
            for (int j = 0; j < 5; j++) {
                System.out.print("*");
            }
            System.out.println();
        }
    }
}
```
오른쪽으로 기울어진 별 삼각형 만들기  
```
public class _08_NestedLoop2 {
    public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
            for (int j = 0; j < 4 - i; j++) {
                System.out.print(" ");
            }
            for (int k = 0; k < i; k++) {
                System.out.print("*");
            }
            System.out.println();
        }
    }
}
```
구구단 표 만들기  
```
public class _09_MultipleTable {
    public static void main(String[] args) {
        for (int i = 2; i < 10; i++) {
            for (int j = 1; j < 10; j++) {
                System.out.println(i + " * " + j + " = " + (i * j));
            }
            System.out.println();
        }
    }
}
```
## ✅break 문은 반복문이나 switch문에서 사용되어, 해당 블록을 즉시 종료시키는 명령어  

```
for (int i = 1; i <= 10; i++) {
    if (i == 5) {
        break; // i가 5가 되면 반복 종료
    }
    System.out.println(i);
}
```
## ✅continue 문은 반복문 안에서 사용되며, 현재 반복을 건너뛰고 다음 반복으로 넘어가게 하는 제어문  
```
public class ContinueExample {
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            if (i == 3) {
                continue; // i가 3이면 아래 코드 실행하지 않고 다음 반복
            }
            System.out.println(i);
        }
        System.out.println("끝!");
    }
}
```
While문에서의 Continue  
```
public class ContinueWhile {
    public static void main(String[] args) {
        int i = 0;
        while (i < 5) {
            i++;
            if (i == 2) {
                continue; // i가 2일 때는 출력 생략
            }
            System.out.println(i);
        }
    }
}
```

