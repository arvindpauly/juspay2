# juspay2

import java.util.Arrays;
import java.util.Scanner;

public class juspay2 {
	public static void main(String[] args) {
		Scanner a = new Scanner(System.in);
		System.out.println("enter the  number of strings");
		int num = a.nextInt();
		String[] array = new String[num];
		System.out.println("enter the string");
		for (int i = 0; i < num; i++) {
			array[i] = a.next();

		}
		Arrays.sort(array);
		System.out.println("enter the string to find");
		String s2 = a.next();
		String[] array2 = new String[num];
		int k = 0;
		for (int i = array.length - 1; i >= 0; i--) {
			array2[k++] = array[i];

		}

		int index = 0;
		for (int i = 0; i < num; i++) {
			if (array2[i].equals(s2)) {
				index = i;
				break;
			}
		}
		System.out.println(index);

	}
}
