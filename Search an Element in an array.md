# Search an Element in an array

![1](https://user-images.githubusercontent.com/66235628/86349958-8e26d700-bc7f-11ea-8a11-b0a24ddd10ad.png)

# Solution :
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
	     for(int i=0;i<n;i++)
	     {
	         arr[i]=scan.nextInt();
	     }
	     int x=scan.nextInt();
	     int index=-1;
	     for(int i=0;i<n;i++)
	     {
	         if(x==arr[i])
	         {
	             index=i;
	             break;
	         }
	     }
	     System.out.println(index);
	     
	     t--;
	 }
	 }
}
