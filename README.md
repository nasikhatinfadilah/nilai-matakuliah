package nilaimatkul;

import java.util.Scanner;
public class NilaiMatkul {

    public static void main(String[] args) {
        String nama, nim;
        int banyak, angka[], i, max, min;
        angka=new int[100];
        float rata, total=0;
        
            Scanner input= new Scanner(System.in);
            System.out.println("nama:");
            nama= input.next();
            System.out.println("nim: ");
            nim=input.next();
            System.out.print("berapa nilai yang akan diinputkan: ");
            banyak=input.nextInt();
            
            for(i=1;i<=banyak;i++)
            {
                System.out.println("nilai ke- :"+i+" :");
                angka[i] = input.nextInt();
                 total = total + angka[i];
            }
            max=angka[1];
            for(i=1; i<=banyak; i++)
            {
                if(angka[i]>max){
                 max=angka[i];
                 }
            }
            min=angka[1];
             for(i=1; i<=banyak; i++){
                if(angka[i]<min){
                min=angka[i];
            }
            }
                    System.out.println("\nnama: "+nama);
                    System.out.println("nim: "+nim);
                    System.out.println("Nilai Terkecilnya adalah : "+min);
                    System.out.println("Nilai makasimum adalah : "+max);
                    rata = total/banyak;
                    System.out.println("Hasil rata-rata adalah : " + rata);

           
    }
    
}
