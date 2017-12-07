package diziler;

import java.util.Scanner;

public class dizilerornek2 {

	public static void main(String[] args) {
		int boyut=5;
		Scanner input=new Scanner(System.in);
		int[]dizi2=new int[boyut];
		for(int i=0; i<dizi2.length; i++)
		{
			dizi2[i]=(int)(Math.random()*(dizi2.length));
		}
		for(int i=0; i<dizi2.length; i++)
		{
			System.out.println((i+1)+ " = " + dizi2[i] +", ");
		}
		int toplam=0;
		for(int i=0; i<dizi2.length; i++)
		{
			toplam=toplam + dizi2[i];
			
		}
		System.out.println("sayıların toplamı="+toplam);
		
		int min=dizi2[0];
		for(int i=1; i<dizi2.length;i++)
		{
			if(dizi2[i]<min)
			{
				min=dizi2[i];
			}
				
		}
		System.out.println("min="+min);
		
		int max=dizi2[0];
		for(int i=1; i<dizi2.length; i++)
		{
			if(dizi2[i]>max)
			{
				max=dizi2[i];
			}
		}
		System.out.println("max="+max);
		//ortalama hesaplama da çıkar..........
	}
	

}
