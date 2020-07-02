# Searching a number
![1](https://user-images.githubusercontent.com/66235628/86351313-b31c4980-bc81-11ea-8cca-82a2e70823fe.png)

# Solution :
~~~java

import java.util.*;
import java.lang.*;
import java.io.*;
class GFG
 {
static int arr[] = new int[1000000];
    public static int linearSearch(int N, int K) {
        
        // Iterate forward through each element in the given arr[]
        // Once we have a match with the key then we return that elements index within the arr[]
        for (int i=0; i < N; i++) {
            if (arr[i] == K)
                return i+1; // not using 0-base indexing for this problem I guess so add one 
        }
        // Else return -1 if the element is not present in arr[]
        return -1;
    }

    public static void main (String[] args) throws IOException {
        
        BufferedReader reader = new BufferedReader(new InputStreamReader(System.in));
        int T = Integer.parseInt(reader.readLine());
        while (T-- > 0) {
            String str[] = reader.readLine().trim().split("\\s+"); // first testcase arr[]
            int N = Integer.parseInt(str[0]); //number of elements in arr[]
            int K = Integer.parseInt(str[1]); // search key
            String strT[] = reader.readLine().trim().split("\\s+"); // second test case arr[]
            
            for (int i=0; i < N; i++) {
                try {
                    arr[i] = Integer.parseInt(strT[i]);
                } catch (NumberFormatException nfe) {
                    nfe.printStackTrace();
                }
            }
            System.out.println(linearSearch(N, K));
        }
	 }
}
