![Annotation 2020-07-02 013640](https://user-images.githubusercontent.com/66235628/86286667-84ac5900-bc04-11ea-936e-d9ec6b7cfabe.png)

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
	     for(int i=0;i<n;i++)
	     {
	         arr[i]=scan.nextInt();
	     }
	     for(int i=n-1;i>=0;i--)
	     {
	     System.out.print(arr[i]+" ");
	     }
	     System.out.println();
	     
	     t--;
	 }
	 }
}
