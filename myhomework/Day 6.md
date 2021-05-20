- hw1
```java
package homework;

import java.util.Scanner;

public class Day6_hw_1 {

	public static void main(String[] args) {
		
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();	
		
		int sum = 0;
		int num = 0;
		
		for (int i = 0; sum < n; i++) {
			if (i % 2 == 1) {
				sum = sum + i;
				num++;
			}
		}
		System.out.println(sum);
		System.out.println(num);

	}

}
```

- hw2
```java
package homework;

import java.util.Scanner;

public class Day6_hw_2 {

	public static void main(String[] args) {
		
		Scanner sc = new Scanner(System.in);
		
		System.out.println("수를 입력하세요");
		
		int n = sc.nextInt();
		
		int line = n + (n-1);
		int star = n + (n-1);
		int space = line /2 - 2;
		
		for (int i = 0; i < line; i++) {
			for (int j = 0; j < space; j++) {
				System.out.print(" ");
			}
			for (int j = 0; j < star; j++) {
				System.out.print("*");
			}
			if (i < line/2) {
				star = star - 2;
				space = space + 1;
			} else {
				star = star + 2;
				space = space - 1;
			}
			System.out.println();
		}
	}

}
```

- hw3
```java
package homework;

import java.util.Scanner;

public class Day6_hw_3 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int line = sc.nextInt();

		int num = 1;
		for (int i = 0; i < line; i++) {
			for (int j = 0; j < line; j++) {
				System.out.print(num + " ");
				num = num + 2;
				if (10 <= num)
					num = 1;
			}
			System.out.print('\n');
		}
	}
}
```
