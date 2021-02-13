# Printing no of occurance of every letter in string



import java.util.*;
public class OccuranceChar
{
	public static void Stroccur(String s)
	{
		int j=0;
		while(j < s.length()) //iterating string and checking index of string 
		{
			int res = 0;
			char chr = s.charAt(j); // value present at " j " will copy to chr letter
			System.out.print(chr); 
			for (int i = 0; i < s.length(); i++) // iterating string 
			{
				if(s.charAt(i) == chr) // comparing value at index " i " with " chr " if it get match incrementing the counter
				{
					res++;	
					j++;	// 				
				}
			}System.out.print("-" + res + "\t"); // printing the counter 
		}
	}
	public static void main(String[] args)
	{
		Scanner sc = new Scanner(System.in); // creation of object
		String str = sc.nextLine(); // taking string from user
		System.out.println("Entered String is "+ str);
		Stroccur (str); // function call
	}

