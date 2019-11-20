using system;

public class PalindromeStringExample
	{
    public static void Main(string[] args)
    {
       string s, revs = "";
       Console.WriteLine("Purpose of this Program");
       Console.WriteLine("To Find if a String is a Palindrome or not");
       Console.WriteLine("Please Enter a string: ");
       s = Console.ReadLine();
       s = s.Trim();
       for (int i = s.Length - 1; i >= 0; i--)
       {
          revs += s[i].ToString();
       }
       if (revs == s)
       {
          Console.WriteLine("String is a Palindrome \n You have Entered the Following String {0} \n and the reverse string is {1}", s, revs);
       }
       else
       {
          Console.WriteLine("String is not a Palindrome \n You have Entered the Following String {0} \n and the reverse string is {1}", s, revs);
       }

    }
}
