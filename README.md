# Loca-TPS
public class main {
    static int a;
    static int b;


    public static  int generate(int g) {
        a =(int)(Math.random() * 10) ;
        System.out.println("il target : "+a);
        for(int i = 1;i<=a;i++){
            System.out.println(i);
        }
        return a;
    }

    public static void revert(int reSO){
        b= (int)(Math.random() * a) ;
        System.out.println("ciao "+b);
        for(int y =a;y!=b;y--){
            System.out.println(y);
        }System.out.println(b);
    }
    public static void reset(){

    }
    public static void main(String[] args) throws InterruptedException {
        Thread.sleep(1000);
        int rev=0;
        do{
            generate(a);

            revert(rev);


        }while(rev==0);




    }
}
