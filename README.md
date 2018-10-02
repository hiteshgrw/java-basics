# java-basics
program on use array in java
package com.company;

import java.util.Scanner;

public class q1 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("ENTER THE SIZE OF THE ARRAY :");
        int size =sc.nextInt();
        int [] nums = input(size);
        int max = nums[0];
        for (int i = 0; i <size ; i++)
        {
          if(max<nums[i])
              max=nums[i];
        }
        System.out.println("THE MAXIMUM VALUE OF THE ARRAY IS :"+max);
    }
    public static int[] input(int s)
    {
        Scanner sc = new Scanner(System.in);
        int [] data=new int[s];
        for (int i = 0; i <s ; i++)
        {
            data[i]=sc.nextInt();
        }
        return data;
    }
}

