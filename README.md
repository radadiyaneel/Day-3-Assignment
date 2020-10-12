# Day-3-Assignment
package com.marksheet;
import java.util.Scanner;



public class Main {

    public static void main(String[] args) {

        float eng, math, che, phy, cs;
        double per, avg, tot;
        char grade;

        Scanner op = new Scanner(System.in);
        System.out.println("Enter Marks of five subjects");
        System.out.println("Enter English Marks");
        eng = op.nextFloat();
        System.out.println("Enter Maths Marks");
        math = op.nextFloat();
        System.out.println("Enter Chemistry Marks");
        che = op.nextFloat();
        System.out.println("Enter Physics Marks");
        phy = op.nextFloat();
        System.out.println("Enter Computer Science Marks");
        cs = op.nextFloat();

        tot = eng + math + che + phy + cs;
        per = (tot / 500.0) * 100;
        avg = tot / 5.0;

        if (per>=90 && per<100)
        {
            System.out.println( grade = 'A');
            System.out.println(per);
        }
        else if (per>=80 && per<90)
        {
            System.out.println(grade = 'B');
            System.out.println(per);
        }
        else if (per>=60 && per<80)
        {
            System.out.println(grade = 'C');
            System.out.println(per);
        }
        else if (per>=35 && per<60)
        {
            System.out.println(grade = 'D');
            System.out.println(per);
        }
        else
        {
            System.out.println("You have not cleared the exam.");
            System.out.println(per);
        }
    }
}
