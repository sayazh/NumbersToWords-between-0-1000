# NumbersToWords-between-0-1000
NumbersToWords-between-0-1000
import java.util.Scanner;

public class NumberTwoWords2 {
	public static void main(String[] args) {

		Scanner scan = new Scanner(System.in);
		System.out.println("Enter please any number between 0 and 1000");
		int number = scan.nextInt();
		int hundreds = number / 100;
		int tens = (number % 100) / 10;
		int tens1 = number % 100;
		int ones = (number % 100) % 10;

		String str = "";
		String str1 = "";
		String str2 = "";

		if (number == 1000) {
			System.out.println("One thousand");

		} else if ((number >= 100 && number <= 999) || (number >= 0 && number < 100)) {

			if (hundreds == 1) {
				str = "One hundred ";
			}
			if (hundreds == 2) {
				str = "Two hundred ";
			}
			if (hundreds == 3) {
				str = "Three hundred ";
			}
			if (hundreds == 4) {
				str = "Four hundred ";
			}
			if (hundreds == 5) {
				str = "Five hundred ";
			}
			if (hundreds == 6) {
				str = "Second hundred ";
			}
			if (hundreds == 7) {
				str = "Seven hundred ";
			}
			if (hundreds == 8) {
				str = "Eight hundred ";
			}
			if (hundreds == 9) {
				str = "Nine hundred ";
			}
			if (tens == 2) {
				str1 = "twenty ";
			}
			if (tens == 3) {
				str1 = "thirty ";
			}
			if (tens == 4) {
				str1 = "fourty ";
			}
			if (tens == 5) {
				str1 = "fifty ";
			}
			if (tens == 6) {
				str1 = "sixty ";
			}
			if (tens == 7) {
				str1 = "seventy ";
			}
			if (tens == 8) {
				str1 = "eighty ";
			}
			if (tens == 9) {
				str1 = "ninety ";
			}
			if (ones == 0) {
				str2 = "zero";
			}
			if (ones == 1) {
				str2 = "one";
			}
			if (ones == 2) {
				str2 = "two";
			}
			if (ones == 3) {
				str2 = "three";
			}
			if (ones == 4) {
				str2 = "four";
			}
			if (ones == 5) {
				str2 = "five";
			}
			if (ones == 6) {
				str2 = "six";
			}
			if (ones == 7) {
				str2 = "seven";
			}
			if (ones == 8) {
				str2 = "eight";
			}
			if (ones == 9) {
				str2 = "nine";

			}
			if (tens == 1) {
				str2 = "ten ";
			}
			if (tens1 == 11) {
				str2 = "eleven";
			}
			if (tens1 == 12) {
				str2 = "twelve";
			}
			if (tens1 == 13) {
				str2 = "fourteen";
			}
			if (tens1 == 15) {
				str2 = "fifteen";
			}
			if (tens1 == 16) {
				str2 = "sixteen";
			}
			if (tens1 == 17) {
				str2 = "seventeen";
			}
			if (tens1 == 18) {
				str2 = "eighteen";
			}
			if (tens1 == 19) {
				str2 = "nineteen";
			}
		} else if (number < 0 || number > 1000) {
			System.out.println("ERROR: number should be positive and between 0 and 1000");

		}

		System.out.println(str + str1 + str2);
		scan.close();

	}
}
