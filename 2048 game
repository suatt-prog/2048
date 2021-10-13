package oyun2;

import java.util.Random;
import java.util.Scanner;
import static oyun2.Oyun2.tablo;

public class Oyun2 {
    static int tablo [][]={{0,0,0,0,0},{0,2,2,0,0},{0,2,0,2,0},{0,0,2,0,0},{0,0,0,0,0}};
    public static void main(String[] args) {
        Random su = new Random();
        System.out.println(su);
        Scanner s = new Scanner(System.in);
        int a = -1;
        for(int q=1;q<4;q++){
            for(int p=1;p<4;p++){
                System.out.print(tablo[q][p]);
            }
            System.out.println("");
        }
        while (a!=0){
           System.out.println("Sağa kaydırmak için 3 e sola kaydırmak için 1 e aşağı kaydırmak için 2 ye yukarı kaydırmak için 5 e basıp Entera basınız");
           System.out.println("Oyunu bitirmek için 0 a sonra Entera basınız");
           a=s.nextInt();
           if(a==5){
               yukari();
           }
           if(a==2){
               asagi();
           }
           if(a==3){
            sag();
           }
           if(a==1){
            System.out.println("fbewlfşw");
            sol();
        }
    }
}
    public static void sag(){
        int koyuldu=1;
        for(int y=1;y<4;y++){
            int r=2;
            int hareket=1;
            if(tablo[y][3]==0 && tablo[y][2]==0 && tablo[y][1]!=0 && hareket==1){
                tablo[y][3]=tablo[y][1];
                tablo[y][1]=0;
                if(koyuldu==1){
                    tablo[y][1]=2;
                }
                koyuldu=0;
                hareket=0;
            }
            else if(tablo[y][r]!=0 && tablo[y][r+1]==0 && hareket==1){
                tablo[y][r+1]=tablo[y][r];
                tablo[y][r]=tablo[y][r-1];
                tablo[y][1]=0;
                if(tablo[y][3]==tablo[y][2]){
                    tablo[y][3]=tablo[y][3]*2;
                    tablo[y][2]=0;
                }
                if(koyuldu!=0){
                    tablo[y][r-1]=2;
                    koyuldu=0;
                }
                hareket=0;
            }
            else if(tablo[y][1]==tablo[y][3] && tablo[y][2]==0 && hareket==1){
                tablo[y][3]=tablo[y][3]*2;
                tablo[y][1]=0;
                if(koyuldu!=0){
                    tablo[y][1]=2;
                }
                koyuldu=0;
                hareket=0;
            }
            else if(tablo[y][r]==tablo[y][r+1] && tablo[y][r]!=0 && hareket==1){
                tablo[y][r+1]=2*tablo[y][r+1];
                tablo[y][r]=tablo[y][r-1];
                tablo[y][1]=0;
                if(koyuldu!=0){
                    tablo[y][r-1]=2;
                }
                hareket=0;
                koyuldu=0;
            }
            else if(tablo[y][2]==0 && tablo[y][1]!=0 && hareket==1){
                tablo[y][2]=tablo[y][1];
                tablo[y][1]=0;
                if(koyuldu!=0){
                    tablo[y][1]=2;
                }
                koyuldu=0;
                hareket=0;
            }
            else if(tablo[y][1]==tablo[y][2] && hareket==1){
                tablo[y][2]=2*tablo[y][2];
                tablo[y][1]=tablo[y][0];
                tablo[y][1]=0;
                hareket=0;
                if(koyuldu!=0){
                    tablo[y][1]=2;
                }
                koyuldu=0;
            }
        koyuldu=0;
        }
        for(int o=1;o<4;o++){
            for(int u=1;u<4;u++){
                System.out.print(tablo[o][u]);
            }
            System.out.print("    "+(o)+".satır   "+"\n");
        }
    }
    public static void sol(){
        int koyuldusol=1;
            for(int y=1;y<4;y++){
            int r=2;
            int hareketsol=1;
            if(tablo[y][1]==0 && tablo[y][2]==0 && tablo[y][3]!=0 && hareketsol==1){
                tablo[y][1]=tablo[y][3];
                tablo[y][3]=0;
                if(koyuldusol==1){
                    tablo[y][3]=2;
                }
                koyuldusol=0;
                hareketsol=0;
            }
            else if(tablo[y][2]!=0 && tablo[y][1]==0 && hareketsol==1){
                tablo[y][1]=tablo[y][r];
                tablo[y][2]=tablo[y][3];
                tablo[y][3]=0;
                if(tablo[y][1]==tablo[y][2]){
                    tablo[y][1]=tablo[y][1]*2;
                    tablo[y][2]=0;
                }
                if(koyuldusol!=0){
                    tablo[y][3]=2;
                    koyuldusol=0;
                }
                hareketsol=0;
            }
            else if(tablo[y][3]==tablo[y][1] && tablo[y][2]==0 && hareketsol==1){
                tablo[y][1]=tablo[y][1]*2;
                tablo[y][3]=0;
                if(koyuldusol!=0){
                    tablo[y][3]=2;
                }
                koyuldusol=0;
                hareketsol=0;
            }
            else if(tablo[y][r]==tablo[y][1] && tablo[y][r]!=0 && hareketsol==1){
                tablo[y][1]=2*tablo[y][1];
                tablo[y][r]=tablo[y][3];
                tablo[y][3]=0;
                if(koyuldusol!=0){
                    tablo[y][3]=2;
                }
                hareketsol=0;
                koyuldusol=0;
            }
            else if(tablo[y][2]==0 && tablo[y][3]!=0 && hareketsol==1){
                tablo[y][2]=tablo[y][3];
                tablo[y][3]=0;
                if(koyuldusol!=0){
                    tablo[y][3]=2;
                }
                koyuldusol=0;
                hareketsol=0;
            }
            else if(tablo[y][3]==tablo[y][2] && hareketsol==1){
                tablo[y][2]=2*tablo[y][2];
                tablo[y][3]=tablo[y][4];
                tablo[y][3]=0;
                hareketsol=0;
                if(koyuldusol!=0){
                    tablo[y][3]=2;
                }
                koyuldusol=0;
            }
        }
        for(int o=1;o<4;o++){
            for(int u=1;u<4;u++){
                System.out.print(tablo[o][u]);
            }
            System.out.print("    "+(o)+".satır   "+"\n");
        }
    }
    public static void yukari(){
        int koyulduyukari=1;
            for(int y=1;y<4;y++){
            int r=2;
            int hareketyukari=1;
            if(tablo[1][y]==0 && tablo[2][y]==0 && tablo[3][y]!=0 && hareketyukari==1){
                tablo[1][y]=tablo[3][y];
                tablo[3][y]=0;
                if(koyulduyukari==1){
                    tablo[3][y]=2;
                }
                koyulduyukari=0;
                hareketyukari=0;
            }
            else if(tablo[2][y]!=0 && tablo[1][y]==0 && hareketyukari==1){
                System.out.println("sex");
                tablo[1][y]=tablo[2][y];
                tablo[2][y]=tablo[3][y];
                tablo[3][y]=0;
                if(tablo[1][y]==tablo[2][y]){
                    tablo[1][y]=tablo[1][y]*2;
                    tablo[2][y]=0;
                }
                if(koyulduyukari!=0){
                    tablo[3][y]=2;
                    koyulduyukari=0;
                }
                hareketyukari=0;
            }
            else if(tablo[3][y]==tablo[1][y] && tablo[2][y]==0 && hareketyukari==1){
                tablo[1][y]=tablo[1][y]*2;
                tablo[3][y]=0;
                if(koyulduyukari!=0){
                    tablo[3][y]=2;
                }
                koyulduyukari=0;
                hareketyukari=0;
            }
            else if(tablo[2][y]==tablo[1][y] && tablo[2][y]!=0 && hareketyukari==1){
                tablo[1][y]=2*tablo[1][y];
                tablo[2][y]=tablo[3][y];
                tablo[3][y]=0;
                if(koyulduyukari!=0){
                    tablo[3][y]=2;
                }
                hareketyukari=0;
                koyulduyukari=0;
            }
            else if(tablo[2][y]==0 && tablo[3][y]!=0 && hareketyukari==1){
                tablo[2][y]=tablo[3][y];
                tablo[3][y]=0;
                if(koyulduyukari!=0){
                    tablo[3][y]=2;
                }
                koyulduyukari=0;
                hareketyukari=0;
            }
            else if(tablo[3][y]==tablo[2][y] && hareketyukari==1){
                tablo[2][y]=2*tablo[2][y];
                tablo[3][y]=tablo[4][y];
                tablo[3][y]=0;
                hareketyukari=0;
                if(koyulduyukari!=0){
                    tablo[3][y]=2;
                }
                koyulduyukari=0;
            }
        }
        for(int o=1;o<4;o++){
            for(int u=1;u<4;u++){
                System.out.print(tablo[o][u]);
            }
            System.out.print("    "+(o)+".satır   "+"\n");
        }
    }
    public static void asagi(){
        int koyulduasagi=1;
        for(int y=1;y<4;y++){
            int r=2;
            int hareketasagi=1;
            if(tablo[3][y]==0 && tablo[2][y]==0 && tablo[1][y]!=0 && hareketasagi==1){
                tablo[3][y]=tablo[1][y];
                tablo[1][y]=0;
                if(koyulduasagi==1){
                    tablo[1][y]=2;
                }
                koyulduasagi=0;
                hareketasagi=0;
            }
            else if(tablo[2][y]!=0 && tablo[3][y]==0 && hareketasagi==1){
                tablo[3][y]=tablo[2][y];
                tablo[r][y]=tablo[1][y];
                tablo[1][y]=0;
                if(tablo[3][y]==tablo[2][y]){
                    tablo[3][y]=tablo[3][y]*2;
                    tablo[2][y]=0;
                }
                if(koyulduasagi!=0){
                    tablo[1][y]=2;
                    koyulduasagi=0;
                }
                hareketasagi=0;
            }
            else if(tablo[1][y]==tablo[3][y] && tablo[2][y]==0 && hareketasagi==1){
                tablo[3][y]=tablo[3][y]*2;
                tablo[1][y]=0;
                if(koyulduasagi!=0){
                    tablo[1][y]=2;
                }
                koyulduasagi=0;
                hareketasagi=0;
            }
            else if(tablo[2][y]==tablo[3][y] && tablo[2][y]!=0 && hareketasagi==1){
                tablo[3][y]=2*tablo[3][y];
                tablo[2][y]=tablo[1][y];
                tablo[1][y]=0;
                if(koyulduasagi!=0){
                    tablo[1][y]=2;
                }
                hareketasagi=0;
                koyulduasagi=0;
            }
            else if(tablo[2][y]==0 && tablo[1][y]!=0 && hareketasagi==1){
                tablo[2][y]=tablo[1][y];
                tablo[1][y]=0;
                if(koyulduasagi!=0){
                    tablo[1][y]=2;
                }
                koyulduasagi=0;
                hareketasagi=0;
            }
            else if(tablo[1][y]==tablo[2][y] && hareketasagi==1){
                tablo[2][y]=2*tablo[2][y];
                tablo[1][y]=tablo[0][y];
                tablo[1][y]=0;
                hareketasagi=0;
                if(koyulduasagi!=0){
                    tablo[1][y]=2;
                }
                koyulduasagi=0;
            }
        koyulduasagi=0;
        }
        for(int o=1;o<4;o++){
            for(int u=1;u<4;u++){
                System.out.print(tablo[o][u]);
            }
            System.out.print("    "+(o)+".satır   "+"\n");
        }
    }
}
