# Bubble-Sort-using-Java

/**
 * Write a description of class Bubblesort here.
 *
 * @author (your name)
 * @version (a version number or a date)
 */
public class Bubblesort
{
    // instance variables - replace the example below with your own
    public static void Printarr(int arr[])
    {
         int n=arr.length;
        for(int i=0;i<n;i++)
        {
            System.out.print(arr[i]);
        }
    }
    public static void Sortarr(int arr[])
    {
        int n=arr.length;
        for(int i=0;i<n-1;i++)
        {
            for(int j=0;j<n-1-i;j++)
            {
                if(arr[j]>arr[j+1])
                {
                int temp=arr[j];
                arr[j]=arr[j+1];
                arr[j+1]=temp;
            }
        }
        }
    }
    public static void main(String[] args)
    {
        int arr[]={3,2,5,6,1};
       
        Sortarr(arr);
         Printarr(arr);
    }
}
