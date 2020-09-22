# 1D-array
public class Main
{


public static int[] runningSum(int[] nums)
{
int sum=0;
int size;   
size=nums.length;
int[] newArray= new int[size];


for(int i=0;i<size;i++)
{
sum=sum+nums[i];
newArray[i]=sum;
}
return newArray;
}

public static void main(String[] args) {
int[] nums={1, 2, 3, 4};

int[] newArray= runningSum(nums);

for(int i=0;i<newArray.length;i++)
{
System.out.print(newArray[i]+" ");
}
}
}
