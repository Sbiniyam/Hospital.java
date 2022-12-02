# Hospital.java
import java.util.Scanner;

public class Hospital {
    Scanner scan = new Scanner(System.in);

    String askDirection;
    String cardRoom;
    String appointment;
     void direction (String askDirection){

        if (askDirection.equalsIgnoreCase("pharmacy"))
        System.out.println("The pharmacy is in block 4. \n to get block 4" );
        if(askDirection.equalsIgnoreCase("Laboratory"))
            System.out.println("Laboratory is on block 8");
        if (askDirection.equalsIgnoreCase("Emergency room"))
            System.out.println("Emergency room is on block 9");
    }
    void cardRoomService(String cardRoom) {
        System.out.println("Are you new patient? (Yes/No)");
        if (cardRoom.equalsIgnoreCase("Yes")) {
            System.out.println("Go to room 5");
        } else if ((cardRoom.equalsIgnoreCase("No"))) {
            System.out.println("Go to room 6");
        } else
            System.out.println("Please insert Yes/No");
    }
    void appointmentService(String appointment) {
        System.out.println("Do you have appointment with your doctor? (Yes/No)");
        if (appointment.equalsIgnoreCase("Yes")) {
            System.out.println("With whom do you have appointment? Dr. Sara or Dr. Abel?");
            String doctorName = scan.nextLine();
            if (doctorName.equalsIgnoreCase("Dr. sara")) {
                System.out.println("Go to room 12");
            } else if (doctorName.equalsIgnoreCase("Dr. Abel")) {
                System.out.println("Go to room 14");
            } else {
                System.out.println("Please insert your answer like 'Dr. Sara or Dr. Abel' ");

            }

        } else
            System.out.println("You don't have appointment");
    }


    }
