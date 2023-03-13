# comman_element_in_two_Array

package homework;
import java.util.*;
public class comman_element_array {
	
	
	Scanner sc = new Scanner(System.in);
	int arr1[]=new int[10];
	int arr2[]=new int[10];
	int comm[]=new int[10];
	
	
	int size;
	
	void Accept()
	{
		System.out.print("Enter Array Size : ");
		size=sc.nextInt();
		
		System.out.println("Enter 1st Array : ");
		for(int i=0;i<size;i++)
		{
			arr1[i]=sc.nextInt();
		}
		
		System.out.println("Enter 2nd Array : ");
		for(int i=0;i<size;i++)
		{
			arr2[i]=sc.nextInt();
		}
	}
	
	void Display()
	{
		for(int i=0;i<size;i++)
		{
			for(int j=0;j<size;j++)
			{
				if(arr1[i]==arr2[j])
				{
					System.out.println(arr1[i]+" ");
				}
			}
		}
		
	}
	
	

	public static void main(String[] args) {
		

		comman_element_array obj = new comman_element_array();
		obj.Accept();
		obj.Display();
	}

}
