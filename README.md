Java.util.Scanner;
Java.util.ArrayList;
Java.util.LinkedList 

public class VirtualAssistant {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Hello! I am your virtual assistant. How can I help you?")
        //Creating our virtual assistant
        while (true) {
            System.out.print("Your request:");
            String input = scanner.nextLine().toLowerCase();

            if (input.contains(Hello")) {
                System.out.println("Hi!");
            } else if (input.contains("Weather")) {
                getWeather();
            } else if (input.contains("news")) {
                getNews();
            } else if (input.contains("time")) {
                getTime();
                } else if(input.contains("your_condition") {
                getTranslate();
                } else if(input.contains(translate"")) {
            } else if (input.contains("exit") || input.contains("goodbye")) {
                System.out.println("Bye! Thank you for contacting me..");
                break;
            } else {
                System.out.println("I'm sorry, I don't understand your request. Please try to formulate it in a different way.");
            }
        }

        scanner.close();
    }

    private static void getWeather() {
        System.out.println("Weather in Moscow: sunny, temperature +20°C");
    }

    private static void getNews() {
        System.out.println("Latest news: ...");
    }

    private static void getTime() {
        java.time.LocalTime currentTime = java.time.LocalTime.now();
        System.out.println("Текущее время: " + currentTime.toString());
    }
}
// Our virtual assistant is ready
