# domain
import java.io.*;
import java.text.ParseException;
import java.util.*;
Class domain2
{
private static void process(String[] arr)
{
System.out.println(Arrays.toString(arr));
}
public static void main(String[]args)
{
Scanner scanner = new Scanner(System.in);
System.out.println("Enter no. Of Students");
int n = Integer.parseInt(scanner.nextLine());
String[] arr=new String[n];
String[] arr2=new String[n];
String[] arr3=new String[n];
int count =0;
for(int i = 0; i < n; i++)
{
System.out.println("Enter student Name"+i+":");
String str = scanner.nextLine();
arr[i]=str;
System.out.println("Enter student id"+i+":");
String str1 = scanner.nextLine();
arr2[i] = str1;
System.out.println("Enter student Id to apply leave:");
String id = scanner.nextLine();
for(int i=0;i<n;i++)
{
String s = arr2[i];
if(s.equalsIgnoreCase(id))
{
System.out.println("Entered student detail to apply leave" + arr[i]+"::"+arr2[i]);
}
}