import java.util.Scanner;

public class zadacha4 {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.println("Колко кв.м е лозето:");
        int kvm = scan.nextInt();
        System.out.println("Колко грозде взимаш от един кв.м:");
        double grozdeZaKvm = scan.nextDouble();
        System.out.println("Колко литра вино трябват:");
        int nyjnoVino = scan.nextInt();
        System.out.println("Колко работници имаш:");
        int rabotnici = scan.nextInt();

        if(kvm < 10 || kvm > 5000) {
            System.out.println("1ви ред е извън позволените лимити [10 - 5000].");
            return;
        }
        if(grozdeZaKvm < 0.00 || grozdeZaKvm > 10.00) {
            System.out.println("2ви ред е извън позволените лимити [0.00 - 10.00].");
            return;
        }
        if(nyjnoVino < 1 || nyjnoVino > 600) {
            System.out.println("3ви ред е извън позволените лимити [1 - 600].");
            return;
        }
        if(rabotnici < 1 || rabotnici > 20) {
            System.out.println("4ви ред е извън позволените лимити [ww - 20].");
            return;
        }

        int grozde = (int) (((kvm * grozdeZaKvm) * 40) / 100);
        System.out.println(grozde);
        double vino = grozde / 2.5;
        double ostVino = vino - nyjnoVino;
        double trqbvaOshte = nyjnoVino - vino;

        if(vino > nyjnoVino) {
            System.out.println("Има достатъчно вино. Има " + vino + " литри.");
            System.out.println("Остават " + ostVino + " литри вино. → " + ostVino / rabotnici + " вино на човек.");
        }
        else {
            System.out.println("Не стига виното! Трябват още " + Math.floor(trqbvaOshte) + " литра вино.");
        }
    }
}
