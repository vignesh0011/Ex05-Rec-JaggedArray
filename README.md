# EX-5 Jagged Array
## Date:
## Aim:
To write a C# program to create a sample CPU usage on a network with 4 nodes using a jagged array.
## Algorithm:
 ### Step 1: 
Create a new Class named cpu.
### Step 2:
Create a jagged array of 4arrays.
```
int[][] array = new int[4][];
```
### Step 3:
Create as many sub-nodes as you wish inside one node of jagged array.
### Step 4:
Give the sample CPU usage in the jagged array.  
### Step 5:
Print the sample CPU usage in the jagged array.
### Step 6:
End of the Program.



## Program:
</br>

```C#
using System;

namespace exp5
{
    class cpu
    {
        public static void Main(String[] args)
        {

            int[][] cpu = new int[4][];

            cpu[0] = new int[5];
            
            cpu[1] = new int[8];
            
            cpu[2] = new int[3];
            
            cpu[3] = new int[4];

            for (int i = 0; i < 4; i++)
            {
            
                for (int j = 0; j < cpu[i].Length; j++)
                {
                
                    cpu[i][j] = i * j + 70;
                    
                }
            }

            for (int i = 0;i < 4; i++)
            {
            
                for(int j=0; j < cpu[i].Length; j++)
                {
                
                   Console.WriteLine("CPU usage at Node {0} is {1}",i,cpu[i][j]);
                   
                }
                
             Console.WriteLine();
             
            }
        }
    }
}
```

</br>
</br>

## Output:
![image](https://github.com/vignesh0011/Ex05-Rec-JaggedArray/assets/53014593/434678df-4385-46ee-9cc0-dabf8a996a19)

## Result:
Thus,C# program to create a sample CPU usage on a network with 4 nodes using a jagged array is executed successfully.
