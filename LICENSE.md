package com.felight.calc1;

public class Calculator {
	public static int div(int num1, int num2) {
		return num1 / num2;
	}

	public static int[] generateEvenNumbers(int from, int to) {
		int[] array = new int[((to - from) / 2) + 1];
		int index = 0;
		for (int i = from; i <= to; i++) {
			if (isEven(i)) {
				array[index] = i;
				index++;
			}
		}
		return array;
	}

	public static int sumOfArray(int[] array) {
		int sum = 0;
		for (int i = 0; i < array.length; i++) {
			sum = sum + array[i];
		}
		return sum;
	}

	public static void printArray(int[] array) {
		for (int i = 0; i < array.length; i++) {
			System.out.println(array[i]);
		}
	}

	public static int[] generateRandomNumbers(int howMany) {
		int[] array = new int[howMany];
		for (int i = 0; i < array.length; i++) {
			array[i] = (int) (Math.random() * 10000);
		}
		return array;
	}

	// Mistakes
	/*
	 * public static int[] generateNaturalNumbers(int[] array){ int[] array =
	 * new int[howMany];
	 * 
	 * return array; }
	 */

	public static int[] generateNaturalNumbers(int howMany) {
		int[] array = new int[howMany];
		for (int i = 0; i < array.length; i++) {
			array[i] = i + 1;
		}
		return array;
	}

	public static int add(int num1, int num2, int num3) {
		int sum = num1 + num2 + num3;
		return sum;
	}

	public static int add(int num1, int num2) {
		int sum = num1 + num2;
		return sum;
	}

	public static boolean isEven(int num) {
		if (num % 2 == 0)
			return true;
		else
			return false;
	}

}
