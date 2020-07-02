# Searching a number
![1](https://user-images.githubusercontent.com/66235628/86351313-b31c4980-bc81-11ea-8cca-82a2e70823fe.png)

# Solution :
~~~java

class GFG {
	public static void main (String[] args) throws IOException {
	    BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
	    String str = br.readLine();
	    int t = Integer.parseInt(str);
	    while(t-->0)
	    {
	        str = br.readLine();
	        String myarr[] = str.split(" ");
	        int n = Integer.parseInt(myarr[0]);
	        int k = Integer.parseInt(myarr[1]);
	        str = br.readLine();
	        myarr = str.split(" ");
	        List<Integer> list = new ArrayList<>();
	        for(String str1 : myarr)
	        list.add(Integer.parseInt(str1));
	        if(list.contains(k))
	        System.out.println(list.indexOf(k)+1);
	        else
	        System.out.println("-1");
	    }
	}
}
