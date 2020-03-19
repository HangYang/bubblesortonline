public class bubbleSort{
    public static int[] bubblesort(int[] a){
        int i, j;
        for (i = 0;i < a.length - 1;i++) {
            for (j = 0; j < a.length - i - 1; j++) {
                if (a[j] > a[j + 1]) {
                    int t = a[j];
                    a[j] = a[j + 1];
                    a[j + 1] = t;
                }
            }
        }
        return a;
    }
    public static void main(String[] args){
        int count = 0;
        int[] a1 = new int[]{70, 61, 72, 83, 38};
        int[] a2 = new int[]{7,2,76,4,99};
        int[] a3 = new int[]{28,9,13,78,19};
        int[] a4 = new int[]{68,84,41,62,18};
        System.out.println("Result: ");
        bubblesort(a1);
        bubblesort(a2);
        bubblesort(a3);
        bubblesort(a4);
        for(int i : a1){
            count++;
            System.out.print(i + " ");
            if (count % 5 == 0){
                System.out.print("\n");
            }
        }
        for(int i : a2){
            count++;
            System.out.print(i + " ");
            if (count % 5 == 0){
                System.out.print("\n");
            }
        }
        for(int i : a3){
            count++;
            System.out.print(i + " ");
            if (count % 5 == 0){
                System.out.print("\n");
            }
        }
        for(int i : a4){
            count++;
            System.out.print(i + " ");
            if (count % 5 == 0){
                System.out.print("\n");
            }
        }
    }
}
