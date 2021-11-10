# react

package Pack;

import java.util.Iterator;
import java.util.Random;
import java.util.Scanner;

/*ex
public class Hello{
	public static void main(String[] args) {
		
	}
}
*/

//ex16
public class Hello{
	public static void main(String[] args) {
		
	}
}



/*ex15
public class Hello{
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		
		if(num % 4 !=0) {
			num = (num /4 +1)*4;
		}
		System.out.println(num);
	}
}

/*ex14
public class Hello{
	public static void main(String[] args) {
		// 100 - 999 사이 숫자 10개를 랜덤하게 출력
		int count = 10; 
		int a[] = new int[count];
		Random r = new Random();
		
		for(int i=0; i<10; i++){
			a[i] = r.nextInt(1000) + 1;  
			for(int j=0; j<i; j++){
				if(a[i] == a[j]){
					i--;
				}
			}
		}
		for(int i=0; i<10; i++){
			System.out.println(a[i]);
		}
		
		
	}
}
*/

/*ex13
public class Hello {
	public static void main(String[] args) {
		
		int input = 12; 
		for (int i = 1; i <= input; i++) {
			System.out.println(fibo(i));
		}
	}

	public static int fibo(int n) {
		if (n <= 1)
			return n;
		else
			return fibo(n - 2) + fibo(n - 1);
	}
	
	
	//피보나치 case2, 시험에 나올 가능성
	
	long a =0, b=1, c;
	for(int i=0; i<10; i++) {
		c = a+b;
		a = b;
		b= c;
		
		System.out.println(c);
	}
}

/*ex12
public class Hello{
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.println(1);
		
		
		int num = sc.nextInt();
		System.out.println(2);
		
		int num2 = new Scanner(System.in).nextInt();
		
		
		//1000ms = 1초
		//sleep(1000);
		
		//send() >> recv()
	}
}

/*ex11
public class Hello {
	public static void main(String[] args) {
		int x =1, y=2;
		for(int i=0; i<7; i++) {
			for(int j=0; j<7; j++) {
				
					System.out.printf((i==x||y==y+2)||(i==x+2||j==y) ? "X ":".");
				
			}System.out.println();
		}
		
	}
}


/*ex10
public class Hello{
	public static void main(String[] args) {
		int w = 6, h = 6;
		int x= 3, y= 3;
		for (int i=0; i<h; i++) {
			for (int j=0;j<w;j++) {
				System.out.print(j==(x+Math.abs(y-i))||j==(x-Math.abs(y-i)) ? "X ":". ");
			} System.out.println();
		}
	}
}

/*ex 9
class Tiger {
	// 생성자, 필드, 메소드
	static void m1() {

	}

	static int num = 100;

}

public class Hello {
	public static void main(String[] args) {

		Hello h = new Hello();
		h.m2();
	}
	static void m1() {
		
	}
	
	void m2() {
		
	}
}

/*ex 8
public class Hello{
	
	static int fl() {
//		if(3>2) {
//			return 100;
//		}else {
//			return 200;
//		}
		return 3>2? 100:200;
		
	}
	
	public static void main(String[] args) {
//		for(int i=4; i>0; i--) {
//			for(int j =3; j>0; j--) {
//				System.out.print(i+"0"+j+" ");
//			}
//			System.out.println();
//		}
		for(int i = 0; i<4; i++) {
			for(int j = 0; j<5; j++) {
				if((i >= 1 && i <= 2) && (j >= 1 && j <= 3))
					//0을 뽑기 위한 조건
					System.out.printf("0 ");
				else
					System.out.printf("* ");
			}System.out.println();
		}
		
	}
}

/*class Hello2{
	public static void main(String[] args) {
		int a;
		if(3>2) {
			a= 10;
		}else {
			a=20;
		}
		a = 3>2? 10:20;
		System.out.println(3>2? "호랑이":"코끼리");
	}
}


/*ex7
public class Hello{
	public static void main(String[] args) {
		for(int i=0; i<3; i++) {
			for(int j=0; j<4; j++) {
				System.out.printf("%02d호 ", (4-i)*j);
			}
			System.out.println();
		}
		
	}
}

/*ex6
public class Hello {
	public static void main(String[] args) {
		// 1)
//		Random rn = new Random();
//		for (int i = 0; i < 4; i++) {
//			int sum = 0;
//			for (int j = 0; j < 3; j++) {
//				int temp = rn.nextInt(10);
//				sum += temp;
//				System.out.printf("%d ", temp);
//			}
//			System.out.printf("%d \n", sum);
//		}
		
		// 2)
		Random rn = new Random();
		for (int i = 0 ; i < 3 ; i++) {
			for(int j = 0 ; j < 4 ; j++) {
				int temp = rn.nextInt(26) + 'A';
				System.out.printf("%c ", (char)temp);
			}
			System.out.println();
		}
		
	}
}

/* ex5 
  public class Hello{ 
 	public static void main(String[] args) { 
 		Random rn = new Random(); 
 		for (int i = 0; i < 10; i++) { 
 		// 0 - 99 
 		 	int num = rn.nextInt(100); 
 		 	System.out.println(num + " "+rn.nextInt(100)); 
 		 	} 
 		 		for (int i = 0; i < 10; i++) {
 		 	 		new Random().nextInt(10); 
 		 	 } 
 		 } 
 	}
 
 * /*ex4 public class Hello{ public static void main(String[] args) { for (int i
 * = 0; i < 3; i++) { for (int j = 0; j < 4; j++) { //offset을 구하는 공식
 * System.out.printf("%2d ",i*4+j); } System.out.println(); }
 * System.out.println("------------------------");
 * 
 * for (int i = 0, k=0; i < 3; i++) { for (int j = 0; j < 4; j++, k++) {
 * System.out.printf("%2d ",k); } System.out.println(); }
 * System.out.println("------------------------"); } }
 * 
 * /*ex3 public class Hello { public static void main(String[] args) { for (int
 * i = 0; i < 3; i++) { for (int j = 0; j < 4; j++) { System.out.println("[" + i
 * + " " + j + "]"); } System.out.println(); }
 * System.out.println("------------------------");
 * 
 * for (int i = 0; i < 3; i++) { for (int j = 0; j < 4; j++) {
 * System.out.printf("[%d,%d]",10,20); } System.out.println(); }
 * System.out.println("------------------------"); }
 * 
 * }
 * 
 * /* ex3 public class Hello{ public static void main(String[] args) { for (int
 * i = 0; i < 3; i++) { for (int j = 0; j < 4; j++) {
 * System.out.println("["+i+" "+j+"]"); } System.out.println(); } } }
 */

/*
 * ex2 public class Hello { public static void main(String[] args) { for (int i
 * = 0; i < 4; i++) { System.out.print(i+" "); }
 * 
 * } }
 */

/*
 * ex1) public class Hello {
 * 
 * public static void main(String[] args) { for (int i = 0; i <4; i++) {
 * System.out.println(i); }
 * 
 * }
 * 
 * }
 */
