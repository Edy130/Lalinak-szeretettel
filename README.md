# Lalinak-szeretettel


import java.util.Scanner;

public class SumOddNumbers {
    public static void main(String[] args) {
        int x, i, sum = 0;
        Scanner input = new Scanner(System.in);
        System.out.println("Enter a number");


        if(input.hasNextInt()) {
            x = input.nextInt();
            for (i = 0; i <= x; ++i) {
                if ((i % 2) == 1) {
                    sum += i;
                }
            }
            System.out.print(sum + " " + "(" +" ");
            if (x % 2 == 1) {
                for (i = 1; i <= x - 2; i++) {
                    if (i % 2 != 0) {
                        System.out.print(i + " " + "+" + " ");
                    }
                }
                System.out.print(x +" " + ")");
            } else {
                for (i = 1; i <= x - 3; i++) {
                    if (i % 2 != 0) {
                        System.out.print(i + " " + "+" + " ");
                    }
                }System.out.print(x-1 + " " + ")");
            }
        }
        else{
            System.out.println("Invalid number");
        }

    }
}
