# artikYil
import java.util.Scanner;

public class main {
    public static void main(String[] args) {
        int year;
        boolean leapYear = false;

        Scanner inp = new Scanner(System.in);
        System.out.print("Yıl giriniz: ");
        year = inp.nextInt();

        if(year % 4 == 0) {
            if (year % 100 == 0) {
                if (year % 400 == 0) {
                    leapYear = true;
                } else {
                }       leapYear = false;
                }
            } else {
                leapYear = true;
            }

            if (leapYear) {
                System.out.println(year + " artık yıldır");
            } else {
                System.out.println(year + " artık yıl değildir");
            }
        }
