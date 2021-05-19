# Day4

- 실습문제 1
```java
public class Ch02_p74 {

	public static void main(String[] args) {
		
		int a = Integer.parseInt(args[0]);
		int b = Integer.parseInt(args[1]);
		int c = Integer.parseInt(args[2]);
		
		int sum = (a + b + c);
		System.out.println("sum" + " : " + sum);
		
		int avg = sum / 3;
		System.out.println("avg" + " : " + avg);
	}

}
```

- 실습문제 2
```java
public class Ch02_day_homework2 {

	public static void main(String[] args) {
		int a = Integer.parseInt(args[0]);
		int b = Integer.parseInt(args[1]);

		System.out.println(a + 100);
		System.out.println(b % 10);		

	}

}
```

- 실습문제 3
```java
public class Ch02_day_homework3 {

	public static void main(String[] args) {
		int a = Integer.parseInt(args[0]);
		int b = Integer.parseInt(args[1]);
		
		System.out.println(a + " / " + b + " = " + (a / b) + " ... " + (a % b));
	}

}
```
