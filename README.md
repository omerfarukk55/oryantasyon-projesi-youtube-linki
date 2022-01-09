# oryantasyon-projesi-youtube-linki
youtube da cözümlü problemler
package omerfaruk;


public class NewClass1 {
    public static void main(String[] args){
    int ct=0;
    int tt=0;
            
    for (int i = 1; i < 100; i=i+2){         
         ct=ct+i;
    }
        for (int j =0; j < 100; j=j+2){
            tt=tt+j;
        }
        System.out.println("tek sayıların toplamı"+tt );
        
        System.out.println("çift sayıların toplamı"+ct );
    
        }
 
}
    package omerfaruk;

/**
 *
 * @author MONSTER
 */
public class switcblok {
    public static void main(String[]arms){
    char grade='e';
    
    switch (grade){
        case 'A':
            System.out.println("gecerli: müthiş");
            break;
        case'B':
            System.out.println("gecerlinot:mükemmel");
            break;
        case'c':
            System.out.println("gecerlinot:iyi");
            break;
         case'd':
             System.out.println("gecerli:orta");
             break;
            
          case'f':
              System.out.println("geçersiznot bokgibi");
             break;
          default:
              System.out.println("yasak nokta.com ");
    
             
    }
     }            
}
package omerfaruk;


public class recapdemo {
   public static void main(String[] args){
       String[][] sehirler =new String[3][3];
       sehirler[0][0] = "istarbul";
       sehirler[0][1] = "bursa";
       sehirler[0][2] = "bilecik";
       sehirler[1][0] = "ankara";
       sehirler[1][1] = "konya";
       sehirler[1][2] = "kayseri";
       sehirler[2][0] = "şanlıurfa";
       sehirler[2][1] = "gaziantep";
       sehirler[2][2] = "adıyaman";
            for(int i=0; i<=2; i++ ){
               System.out.println("------------");
            for(int j=0; j<=2; j++){ 
           
                System.out.println(sehirler[i][j]);
       
       
   }}
             
           
       
         
       
   }
   
    
}package omerfaruk;

/**
 *
 * @author MONSTER
 */
public class buyukkucuksayılar {
    public static void main(String[] args){
        int  sayi1=28;
        int sayi2=29;
        int sayi3=27;
        int enBuyuksayı=sayi1;
        int enkucuksayı=sayi1;
       
        if(enkucuksayı<sayi2){
            enkucuksayı=sayi2;
        }
        if(enkucuksayı>sayi3){
            enkucuksayı=sayi3;
        }
        if (enBuyuksayı<sayi2){
            enBuyuksayı=sayi2;
        } if(enBuyuksayı<sayi3){
            enBuyuksayı=sayi3;
        } 
        System.out.println("en büyük sayı"+enBuyuksayı);
        System.out.println("en kücük sayı"+enkucuksayı);
    }
}
package omerfaruk;

import java.util.Scanner;
public class remainderasalsayı {
    public static void main(String[] args){
        Scanner giris=new Scanner(System.in);
        int number= giris.nextInt();
        
        
        int reminder=number%2;
        System.out.println(reminder);
        boolean isPrime= true;
        if (number==1){
            System.out.println("sayı asaldeğil");
        return; } 
        for (int i=2; i<number; i++){
          if(number%i==0){
              isPrime=false;
          }       
    }
       if(isPrime){
           System.out.println("sayıasaldır");
           
       }else{
           System.out.println("sayı asaldegil");
       }
          
    }
    
}import java.util.Scanner;
public class noktalıSayıjava {
    public static void main(String[] args){
        
        Scanner giris=new Scanner(System.in);
        System.out.println("1 kardeş yaşını giriniz?");
        int kardes1=giris.nextInt();
        System.out.println("2 kardeş yaşını giriniz");
        int kardes2=giris.nextInt();
        int ortalaması=(kardes1+kardes2)/2;
        System.out.println("kardeşsayılarınort="+ortalaması);
        int toplamı=kardes1+kardes2;
        System.out.println("kardeşsayılarının toplamı"+toplamı);
        
       
        
    }
}package omerfaruk; 
 import java.io.IOException;
 import java.text.DecimalFormat;
 import java.util.Scanner;
        

public class omerinlog {
    public static void main(String[] args)throws IOException {
       Scanner giris = new Scanner(System.in);
       double satis, ucret;
      //decimal tipiyle özel biçimlerde sayılar gösterebilirsiniz 
      DecimalFormat nf = new DecimalFormat("###,###,00");
      System.out.println("günlük kac tane sut satıyor? ");
      satis= giris.nextDouble();
       if (satis<50){
           ucret=15.0 + satis*1.0;
       }else{
           ucret= 15.0 + 50*2.0+ (satis-50)*3;
           
       }
        System.out.println("buna göre günlük ücretiniz:"+nf.format(ucret)+"tl");
    }
}package omerfaruk;

import java.util.Scanner;
public class mükemmelsayı {
    //mükemmel sayı 
    // 6= 1+2+3 eşitse bölenler mükemmel sayı 
    public static void main(String[] args){
        Scanner giris=new Scanner(System.in);
          System.out.println("sayı giriniz");
        int number= giris.nextInt();
        int total=0;
        
        for(int i=1; i<number; i++){
            if(number%i==0){
                total=total+i;
             
            }
        }
        if(total==number){
            System.out.println("mükemmelsayı");
        }
        else {
            System.out.println("mükemmelsayı değil");
        }
    }
}import java.util.Scanner;
public class tahminet100ekadar {
    public static void main(String[] args){
       int tahmin=(int)(Math.random()*101);
       Scanner giris=new Scanner(System.in);
        System.out.println("sayı tahmini girini 1 den 100 e kadar"+tahmin);
        int sayım=giris.nextInt();
        while(sayım==tahmin){
            System.out.println("tahmininiz dogrudur "+tahmin);
            break;
        }
        if(sayım>tahmin){
            System.out.println("sayı tahminden büyük "+tahmin);
        }
        else if(sayım<tahmin){
        System.out.println("tahmin büyük sayıdan ");
        
        
    }
       
    }
            
    
   
}
import java.util.Scanner;
public class randomToplama {
    public static void main(String[] args){
        int sayı1=(int)(Math.random()*10);
        int sayı2=(int)(Math.random()*10);
        Scanner giris=new Scanner(System.in);
        System.out.println("1 sayı ile 2 sayı toplamı nedir? "+sayı1+" + "+sayı2+"=?");
        int cevap=giris.nextInt();
        while(sayı1+sayı2!=cevap){
            System.out.println("cevap dogru değil tekrar giriniz");
            cevap=giris.nextInt();
        }
        System.out.println("cevap dogrudur");
    }
    
}
