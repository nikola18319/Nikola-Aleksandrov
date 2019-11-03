import java.util.Scanner;

public class zadacha3 {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.println("Напиши колко почивни дни имаш в година.");
        int holidays = scan.nextInt();
        if(holidays > 365 || holidays < 0) {
            System.out.println("Пичага, в годината има само 365 дни, голямо въображение имаш.");
            return;
        }
        int otherDays = 365-holidays;

        int vremeHolidays = holidays*127;
        int vremeOtherDays = otherDays*63;
        int obshto = vremeHolidays + vremeOtherDays;

        double difference = Math.abs(obshto - 30000);
        double hours = difference / 60;
        double minutes = difference % 60;

        if(obshto >= 30000) {
            System.out.println("Том спи достатъчно.");
            System.out.printf("Но, може да си спестиш време като си играеш %.0f часа и %.0f минути по малко с него.", Math.floor(hours), Math.floor(minutes));
        }
        else {
            System.out.println("Том не спи достатъчно, ще избяга.");
            System.out.printf("Трябва да си играеш %.0f часа и %.0f минути повече с него за да не избагя.", Math.floor(hours), Math.floor(minutes));
        }
    }
}
