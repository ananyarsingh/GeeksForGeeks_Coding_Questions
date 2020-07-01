# Sum of array elements 
![1](https://user-images.githubusercontent.com/66235628/86287234-76127180-bc05-11ea-82f1-787ebcb77f6f.png)
# Solution
~~~java
import java.util.*;
import java.lang.*;
import java.io.*;
class GFG
 {
	public static void main (String[] args)
	 {
	 Scanner scan=new Scanner(System.in);
	 int t=scan.nextInt();
	 while(t!=0)
	 {
	     int n=scan.nextInt();
	     int arr[]=new int[n];
	     int sum=0;
	     for(int i=0;i<n;i++)
	     {
	         arr[i]=scan.nextInt();
	         sum=sum+arr[i];
	     }
	     System.out.println(sum);
	     
	     t--;
	 }
	 }
}
