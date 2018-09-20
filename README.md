# Uppgifter-SI
package exercises;

import java.util.Arrays;
import java.util.Random;

import static java.lang.System.exit;
import static java.lang.System.out;

public class uddArray {
    public static void main(String[] args)  { new uddArray().program(); }

    public void program(){
        int arr[] = new int[]{-9, 3, 0, 4, 9, 18, 5, 5};
        out.println(Arrays.toString(arr));
        udda(arr);
        out.println(Arrays.toString(udda(arr)));

    }


    int [] udda(int[]arr1){
        int u = 0;
        int[] narr = new int[length(arr1)];
        for (int i =0; i < arr1.length; i++){
            if (!(arr1[i] % 2 == 0)){
                narr[u] = arr1[i];
                u++;
            }
        }
        /*for (int i =0; i < arr1.length; i++){
            if (narr[u] % 2 == 1){
                length++;
        }

        }*/
        return narr;
    }


    int length(int[] arr1){
        int length = 0;
        for (int i =0; i < arr1.length; i++){
            if (!(arr1[i] % 2 == 0)){
                length++;
            }
        }
        return length;
    }


}




package samples;
import java.util.Arrays;
import java.util.Random;

import static java.lang.System.exit;
import static java.lang.System.out;
public class maxValue {
    public static void main(String[] args) {new maxValue().program();}

    public void program(){
        double[][] matrice = {
                {-9, 3.5, 4, 2},
                {1, 0, 0, 7},
                {15, -99, 5, 0},
                {4, 4, 4, 1},
                {1, 3, 5, 6}
        };
        out.println(getMax(matrice));


    }
    double getMax(double[][] matrix){
        int row = 0;
        int column = 0;
        double highest = 0;
        for (row = 0; row < matrix.length; row++){
            for ( column = 0; column < matrix.length - 1; column++){
                if (matrix[row][column] > highest){
                    highest = matrix[row][column];
                }
            }
        }
        return highest;
    }


}







package samples;
import java.util.Arrays;
import java.util.Random;

import static java.lang.System.exit;
import static java.lang.System.out;
public class Uppgift3 {
    public static void main(String[] args) { new Uppgift3().program(); }


    public void program(){
    int[] arr1 = {8, 9, 11, 2, 0, -5};
    int[] arr2= {0, 1, 11, 2, 6, -3, -5};
    out.println(Arrays.toString(sammaTal(arr1, arr2)));

    }
    int[] sammaTal(int[] arr1, int[]arr2){
        int[] same = new int[length(arr1, arr2)];
        int j = 0;
        for (int i = 0; i < arr1.length; i++){
            if (arr1[i] == arr2[i]){
                same[j] = arr1[i];
                j++;
            }
        }

        return same;
    }
    int length(int[] arr1, int[]arr2){
        int j = 0;
        for (int i = 0; i < arr1.length; i++){
            if (arr1[i] == arr2[i]){
                j++;
            }
        }

        return j;
    }

}







package exercises;

import samples.Uppgift3;

public class Uppgift5 {
    public static void main(String[] args) {new Uppgift5().program(); }

    public void program(){
        int[] arr1 = {14, 9, 11, 7, 8, 5, 3};



    }


}
