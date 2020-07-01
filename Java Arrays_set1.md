![1](https://user-images.githubusercontent.com/66235628/86286241-c12b8500-bc03-11ea-870f-a81ad273cf81.png)

# Solution
``` java
import java.util.*;
import java.lang.*;
import java.io.*;
class GFG
 {
	public static void main (String[] args)
	 {
	 //System.out.println("Hello GeeksForGeeks");
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
	     double avg=(double)(sum)/n;
	     System.out.printf("%d ",sum);
	     System.out.printf("%.2f\n", avg);
	     
	     t--;
	 }
	 }
}

