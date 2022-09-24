import java.util.Scanner;

public class NotOrtalamasıHesaplama {
    
    public static void main(String[] args) {
        
        int mat,fiz,kim,turk,dil;
        
        Scanner inp = new Scanner(System.in);
        
        System.out.print("Matemetik notunuzu girin: ");
        mat = inp.nextInt();
        
        System.out.print("Fizik notunuzu girin: ");
        fiz =inp.nextInt();
        
        System.out.print("Kimya notunuzu girin: ");
        kim =inp.nextInt();
        
        System.out.print("Türkçe notunuzu girin: ");
        turk =inp.nextInt();
        
        System.out.print("Dil notunuzu girin: ");
        dil =inp.nextInt();
        
        double sonuc = (mat+fiz+kim+turk+dil)/5;
        
        System.out.println("Ortalama Notunuz: "+sonuc);
        
        boolean kosul1 = sonuc>60;
        boolean kosul2 = sonuc<60;
        boolean durum1 = kosul1&&kosul2;
        
        String durum2 = durum1?"Sınıfı Geçtiniz":"Sınıfta Kaldınız";
        
        System.out.println(durum2);       
        
    }
             
        
    }
