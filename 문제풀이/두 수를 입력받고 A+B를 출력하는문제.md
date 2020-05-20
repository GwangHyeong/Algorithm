## 두 수를 입력받고 A+B를 출력하는문제 - 1000
예제 입력 1 2  
예제 출력 3  
### java
~~~~~~
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.util.StringTokenizer;

public class Main1000 {
	 
    public static void main(String[] args) throws NumberFormatException, IOException{ //BufferedReader 로 받을경우 예외처리 해줘야함.
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        StringTokenizer st = new StringTokenizer(br.readLine()); //StringTokenizer인자값에 입력 문자열 넣음
        int a = Integer.parseInt(st.nextToken());
        int b = Integer.parseInt(st.nextToken());
        System.out.print(a+b);
    }
}
~~~~~~

### python
~~~~~~
c = input().split()
a = int(c[0])
b = int(c[1])

print(a+b)
~~~~~~


## 두 수를 입력받고 A+B를 출력하는문제 - 2558
~~~~~~
예제 입력
            1 
            2
예제 출력  
            3 
~~~~~~
### java
~~~~~~
public class Main2558 {

	public static void main(String[] args) throws NumberFormatException, IOException {
		// TODO Auto-generated method stub
		BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
		int a = Integer.parseInt(br.readLine());
		int b = Integer.parseInt(br.readLine());
		int result = a+b;
		System.out.print(result);
	}

}
~~~~~~

### python
~~~~~~
a = int(input())
b = int(input())
result = a + b
print(result)

~~~~~~

## 두 수를 입력받고 A+B를 출력하는문제 - 10953
* 첫째 줄에 테스트 케이스의 개수 T가 주어진다.
* 각 테스트 케이스는 한 줄로 이루어져 있으며, 각 줄에 A와B가 주어진다.

### java
~~~~~~

import java.util.Scanner;

public class Main10953 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		Scanner s = new Scanner(System.in);
		int t = Integer.parseInt(s.nextLine());
		
		for(int i =0; i<t; i++) {
			String arr[] = s.next().split(",");
			System.out.println(Integer.parseInt(arr[0])+Integer.parseInt(arr[1]));
			
		}
		
	}

}
~~~~~~
### python
~~~~~~
t = int(input())
i = 0
while True:
    c = input().split(',')
    a = int(c[0])
    b = int(c[1])
    result = a + b
    i += 1
    print(result)
   
    if i == t:
        break
   

~~~~~~
