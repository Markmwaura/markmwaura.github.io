
### Sorting algorithms  

* 1. Sorting is done in numerical order *
* 2.  Sorting is done using arrays
* 3. Time is an important factor - the algorithm should take the least amount of time to sort a data set.

### 1.Bubble Sort

 This algorithm is mostly suitable  for small data sets.It compares every two elements as it moves across the data set moving horizontally checking which is greater than the other.The aim is to have the least number on the left and the biggest number on the right.


```

public static void main(String []args) {

        int x,y,z,swap;
        Scanner input  = new Scanner(System.in);
        System.out.println("Enter number of integers to sort");
        x= input.nextInt();
        int array[] = new int[x];
        System.out.println("Enter " + x + " integers");
        for(y = 0; y<x;y++)
            array[y]  = input.nextInt();

        for(y = 0 ;y <(x-1);y++){

            for(z = 0;z<x-y-1;z++){

                if(array[z]>array[z+1]){
                    swap = array[z];
                    array[z] = array[z+1];
                    array[z+1] = swap;

                }
            }
        }
        System.out.println("Sorted list members");
        for(y=0;y<x;y++){
            System.out.println(array[y]);
        }


        ```
