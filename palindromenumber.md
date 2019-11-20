using system;

	public class PalindromeExample
	{
	public static void Main(string[] args)
	{
	int number, remainder, sum=0, temp;
	Console.Write("Enter the number: ");
	number = Convert.ToInt32(Console.ReadLine());
	temp = number;
	while(number > 0)
	{
	remainder = number % 10;
	sum = (sum*10) + remainder;
	number = number / 10;
	}
	Console.Write("The Reversed Number of the Original Number is: {0} = ", sum);
	if (temp == sum)
	{
	Console.Write("Number is Palindrome");
	}
	else
	{
	Console.Write("Number is not Palindrome");
	}
	}
}
