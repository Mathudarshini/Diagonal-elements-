

public class Main {
public static void main(String[] args) {
int[][] matrix = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};

   System.out.println("Matrix:");
    printMatrix(matrix);

    System.out.println("Diagonal Elements:");
    printDiagonalElements(matrix);
}

public static void printMatrix(int[][] matrix) {
    for (int i = 0; i < matrix.length; i++) {
        for (int j = 0; j < matrix[0].length; j++) {
            System.out.print(matrix[i][j] + " ");
        }
        System.out.println();
    }
}

public static void printDiagonalElements(int[][] matrix) {
    for (int i = 0; i < matrix.length; i++) {
        System.out.print(matrix[i][i] + " ");
    }
    System.out.println();

    System.out.println("Anti-Diagonal Elements:");
    for (int i = 0; i < matrix.length; i++) {
        System.out.print(matrix[i][matrix.length - i - 1] + " ");
    }
}

}


Output:

Matrix:
1 2 3
4 5 6
7 8 9
Diagonal Elements:
1 5 9
Anti-Diagonal Elements:
3 5 7# Diagonal-elements-
