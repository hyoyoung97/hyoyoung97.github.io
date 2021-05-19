P123

- Q1
```java
package basic1.ch04;

public class Q1If {

	public static void main(String[] args) {
		int num1 = 10;
		int num2 = 20;
		int result = 0;
		
		//위 전체 스캐너 만들
		
		char operater = '+';
		
		if (operater == '+') {
			result = num1 + num2;
		} 
		else if (operater == '-') {
			result = num1 - num2;
		} 
		else if (operater == '*') {
			result = num1 * num2; 
		} 
		else if (operater == '/') {
			result = num1 / num2;
		} 
		else {
			System.out.println("오류입니다.");
		}
		System.out.println("계산값은 " + result + "입니다.");
	}

}
```

- Q2
```java
package basic1.ch04;

public class Q1Switch {

	public static void main(String[] args) {
		int num1 = 10;
		int num2 = 20;
		int result = 0;
		
		char operator = '+'; 
		
		//위 전체 스캐너 만들
		
		switch(operator) {
			case '+' :
				result = num1 + num2;
				break;
			case '-' :
				result = num1 - num2;
				break;
			case '*' :
				result = num1 * num2;
				break;
			case '/' :
				result = num1 / num2;
				break;
			default:
				System.out.println("오류입니다.");
		}
		System.out.println("계산값은 " + result + "입니다.");
	}

}

```

- Q3
```java
package basic1.ch04;

public class Q3 {

	public static void main(String[] args) {
		int i = 1;
		int dan = 6;
		
		for (i=1; i<10; i++) {
			System.out.println(dan + "*" + i + "=" + (dan * i));
			if (i == dan) 			
				break;
		}
	}

}
```

- Q4
```java
package basic1.ch04;

public class Q4 {

	public static void main(String[] args) {
		
		int lineCount = 4;  
		int spaceCount = lineCount/2 +1;
		int starCount = 1;
		
		for(int i = 0; i<lineCount; i++) {
			for(int j = 0; j<spaceCount; j++) {
				System.out.print(' ');
			}
			for(int j=0; j<starCount; j++) {
				System.out.print('*');
			}
			for(int j = 0; j<spaceCount; j++) {
				System.out.print(' ');
			}
			spaceCount-=1;
			starCount+=2;
			System.out.println();
		}
		System.out.println(7%4);
	}
}
```

- Q5
```java
package basic1.ch04;

public class Q5 {

	public static void main(String[] args) {
		int line = 7;
		int space = line / 2;// 왜 1을더해주어할
		int star = 1;

		for (int i = 0; i < line; i++) {
			for (int j = 0; j < space; j++) {
				System.out.print(' ');
			}
			for (int j = 0; j < star; j++) {
				System.out.print('*');
			}
			if (i < line / 2) {
				space = space - 1;
				star = star + 2;
				System.out.println();
			} else {
				space = space + 1;
				star = star - 2;
				System.out.println();
			}

		}
	}

}
```

P100
```java
package basic1.ch04;
 
public class P100alone {
 
	public static void main(String[] args) {
		int score = 50;
		String grade;
		
		if (score>89) {
			grade = "A";
		} else if (score >79) {
			grade = "B";
		} else if (score >69) {
			grade = "C";
		} else if (score >59) {
			grade = "D";
		} else {
			grade = "F";
		}
		System.out.println("Your grade = " + grade);
	}
 
}
```

P106
```java
package basic1.ch04;

public class P106alone {

	public static void main(String[] args) {
		int f = 1;
		String name;
		
		switch(f) {
		
		case 1 : name = "약국";
				break;
		case 2 : name = "정형외과";
				break;
		case 3 : name = "피부과";
				break;
		case 4 : name = "치과";
				break;
		case 5 : name = "헬스클럽";
				break;
		default : name = "존재하지 않는 층";
		}
	System.out.println(f + "층 " + name + "입니다.");
		
	}

}
```

- 비만율 
```java
package basic1.ch04;

import java.util.Scanner;

public class Day5hw1 {

	public static void main(String[] args) {

		Scanner sc = new Scanner(System.in);

		while (true) {
			System.out.println("키와 몸무게 입력하세요.");
			int h = sc.nextInt();
			
			if (h == -1) {
				return;
			} //else
			int w = sc.nextInt();
			int r = w + 100 - h;
			
			if (r > 0) {
				System.out.println(r + " 비만");
			} else {
				System.out.println("비만이 아닙니다.");
			}

		}

	}

}
```

- 비만율 - 삼항연산자
```java
package basic1.ch04;

import java.util.Scanner;

public class Day5hw1_1 {

	public static void main(String[] args) {

		Scanner sc = new Scanner(System.in);

		while (true) {
			System.out.println("키와 몸무게 입력하세요.");
			int h = sc.nextInt();

			if (h == -1) {
				return;
			} // else
			int w = sc.nextInt();
			int r = w + 100 - h;

			String d = (r > 0) ? Integer.toString(r) + "비만" : "비만이 아닙니다.";
			System.out.println(d);
		}
	}

}
```

- 계산기
```java
package basic1.ch04;

import java.util.Scanner;

public class Day5hw2 {

	public static void main(String[] args) {

		Scanner sc = new Scanner(System.in);
		
		int a = sc.nextInt();
		String c = sc.next();
		int b = sc.nextInt();
		
		int d = 0;
		
		switch(c) {
		case "+" :
			d = a + b;
			break;
		case "-" :
			d = a - b;
			break;
		case "*" :
			d = a * b;
			break;
		case "/" :
			d = a / b;
			break;
		} 
		System.out.println(d);

	}

}
```
