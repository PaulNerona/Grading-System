# Grading-System

package com.mycompany.gradingsystem4;
import java.util.Scanner;
public class GradingSystem4 {

    public static void main(String[] args) {
        Scanner input = new Scanner (System.in);              
        String username1 = "Ariane";
        String password1 = "Nulo";
        boolean logIn = false;
        while (!logIn) {
            System.out.println("LOG IN SYSTEM\n");
            System.out.print("Enter a Username: ");
            String uname = input.nextLine();
            System.out.print("Enter a Password: ");
            String pass = input.nextLine();

            if (uname.equals(username1) && pass.equals(password1)) {
                System.out.println("LOG IN SUCCESSFULLY");
                logIn = true;
            } else {
                System.out.println("Invalid Username or Password. Try again");
            }
        }        
        String[] studentNames = {"Aban", "Dela Torre", "Gayanilo", "Hinayon", "Saburao"};
        String[] remarks = new String[]{" ", " ", " ", " ", " "};
        int[] Exam = new int[5];
        int[] Module = new int[5];
        int[] Quiz1 = new int[5];
        int[] Quiz2 = new int[5];
        int[] Quiz3 = new int[5];
        double[] QUIZZES = new double[5];                           
        int[] intQUIZ = new int[5];
        double[] SAS = new double[5];        
        int[] intSAS = new int[5];
        double[] EXAMS = new double[5];        
        int[] intEXAM = new int[5];
        int[] GRADES = new int[5];
        double[] equivalent = new double[5];        
        boolean choseOption1 = false;        
        
        while (true) {
            try {                
                System.out.print("\nMENU \n1. INPUT GRADES \n2. VIEW GRADES \n3. EXIT \n> ");
                int choice = input.nextInt();
                if (choice == 1 && !choseOption1) {                                                                                                                                                        
                        System.out.print("\nQUIZ 1   Score: 0/20 \n");
                        for (int j = 0; j < studentNames.length; j++) {                           
                            String studentName = studentNames[j];
                            int quiz1Score;                           
                            do {
                                System.out.print("Enter " + studentName + " Quiz1 score: ");                           
                                quiz1Score = input.nextInt();
                                if (quiz1Score < 0 || quiz1Score > 20) {                                
                                    System.out.println("Score should be between 0 and 20.");
                                }                            
                            } while (quiz1Score < 0 || quiz1Score > 20);                           
                            Quiz1[j] = quiz1Score;
                        }
                        System.out.print("\nQUIZ 2   Score: 0/30 \n"); 
                        for (int j = 0; j < studentNames.length; j++) {
                            String studentName = studentNames[j];
                            int quiz2Score;
                            do {                               
                                System.out.print("Enter " + studentName + " Quiz2 score: ");
                                quiz2Score = input.nextInt();
                                if (quiz2Score < 0 || quiz2Score > 30) {
                                    System.out.println("Score should be between 0 and 30.");
                                }
                            } while (quiz2Score < 0 || quiz2Score > 30);
                            Quiz2[j] = quiz2Score;
                        }
                        System.out.print("\nQUIZ 3   Score: 0/50 \n");
                        for (int j = 0; j < studentNames.length; j++) {
                            String studentName = studentNames[j];
                            int quiz3Score;
                            do {
                                System.out.print("Enter " + studentName + " Quiz3 score: ");
                                quiz3Score = input.nextInt();
                                if (quiz3Score < 0 || quiz3Score > 50) {
                                    System.out.println("Score should be between 0 and 50.");
                                }
                            } while (quiz3Score < 0 || quiz3Score > 50);
                            Quiz3[j] = quiz3Score;
                        }
                        System.out.print("\nSAS MODULE   Score: 0/100 \n");
                        for (int j = 0; j < studentNames.length; j++) {
                            String studentName = studentNames[j];
                            int moduleScore;
                            do {
                                System.out.print("Enter " + studentName + " SAS Modules score: ");
                                moduleScore = input.nextInt();
                                if (moduleScore < 0 || moduleScore > 100) {
                                    System.out.println("Score should be between 0 and 100.");
                                }
                            } while (moduleScore < 0 || moduleScore > 100);
                            Module[j] = moduleScore;
                        }
                        System.out.print("\nSAS MODULE   Score: 0/100 \n");    
                        for (int j = 0; j < studentNames.length; j++) {
                            String studentName = studentNames[j];
                            int examScore;
                            do {
                                System.out.print("Enter " + studentName + " Exam score: ");
                                examScore = input.nextInt();
                                if (examScore < 0 || examScore > 100) {
                                System.out.println("Score should be between 0 and 100.");
                                }
                            } while (examScore < 0 || examScore > 100);
                            Exam[j] = examScore;
                        }                       
                        for (int j = 0; j < 5; j++) {                            
                            QUIZZES[j] = (Quiz1[j] + Quiz2[j] + Quiz3[j]) * 0.30;                                           
                            intQUIZ = new int[QUIZZES.length];
                            for (int k = 0; k < QUIZZES.length; k++) {                                
                                intQUIZ[k] = (int) Math.round(QUIZZES[k]);                        
                            } 
                        }
                        for (int j = 0; j < 5; j++) {
                            SAS[j] = Module[j] * 0.30;
                            intSAS = new int[SAS.length];
                            for (int k = 0; k < SAS.length; k++) {
                                intSAS[k] = (int) Math.round(SAS[k]); 
                            }
                        }
                        for (int j = 0; j < 5; j++) {
                            EXAMS[j] = Exam[j] * 0.40;
                            intEXAM = new int[EXAMS.length];
                            for (int k = 0; k < EXAMS.length; k++) {
                                intEXAM[k] = (int) Math.round(EXAMS[k]); 
                            }
                        }                                                                   
                        for (int j = 0; j < 5; j++) {
                        GRADES[j] = (intQUIZ[j] + intSAS[j] + intEXAM[j]);
                        }                                                                                                                                                                                                                      
                        for (int j = 0; j < 5; j++) {                                                    
                            if (GRADES[j] >= 50 && GRADES[j] <= 100) {                             
                                remarks[j] = "Passed";                                                   
                                if (GRADES[j] >= 94.8 && GRADES[j] <= 100 ) {
                                equivalent[j] = 1.00;
                                } else if (GRADES[j] >= 89.2 && GRADES[j] <= 94.7) {                                    
                                    equivalent[j] = 1.25;
                                } else if (GRADES[j] >= 83.6 && GRADES[j] <= 89.1) {
                                    equivalent[j] = 1.50;
                                } else if (GRADES[j] >= 78.0 && GRADES[j] <= 83.5) {
                                    equivalent[j] = 1.75;
                                } else if (GRADES[j] >= 72.4 && GRADES[j] <= 77.9) {
                                    equivalent[j] = 2.00;
                                } else if (GRADES[j] >= 66.8 && GRADES[j] <= 72.3) {
                                    equivalent[j] = 2.25;
                                } else if (GRADES[j] >= 61.2 && GRADES[j] <= 66.7) {
                                    equivalent[j] = 2.50;
                                } else if (GRADES[j] >= 55.6 && GRADES[j] <= 61.1) {
                                    equivalent[j] = 2.75;
                                } else {
                                    equivalent[j] = 3.00;
                                }
                            } else {                                
                                remarks[j] = "Failed";                               
                                equivalent[j] = 5.00;                           
                            }
                        }                              
                    choseOption1 = true;    
                    } else if (choice == 1 && choseOption1) {   
                        System.out.println("DONE INPUT THE GRADES!");    
                        
                    } else if (choice == 2) {                  
                        System.out.println("----------------------------------------------------------------------------------------------------------------------------------------------");
                        System.out.println("""
                                                                   PHINMA CAGAYAN DE ORO COLLEGE
                                                                   GRADING SYSTEM
                                                                   QUIZZES 30% + SAS LEARNING MODULES 30% + PERIODICAL EXAM 40%""");                        
                        System.out.println("----------------------------------------------------------------------------------------------------------------------------------------------");
                        System.out.println("PERIODICAL 1 GRADES ");
                        System.out.print("""
                                                                 SUBJECT CODE: GEN 002 - UNDERSTANDING THE SELF
                                                                 INSTRUCTOR: MS. ARIANNE NULO
                                                                 """);
                        System.out.println("+-------------------+---------------------+-------------------------+---------------------+----------------------+-------------------+---------+");
                        System.out.println("|   Student Name    | QUIZ PERCENTAGE 30% | SAS LEARNING MODULE 30% | EXAM PERCENTAGE 40% | PERIODICAL 1 GRADE   | EQUIVALENT GRADE  | REMARKS |");
                        System.out.println("+-------------------+---------------------+-------------------------+---------------------+----------------------+-------------------+---------+");
                        for (int j = 0; j < studentNames.length; j++) {
                        System.out.printf("| %-18s| %-20d| %-24d| %-20d| %-21d| %-18s| %-8s|\n", studentNames[j], intQUIZ[j], intSAS[j], intEXAM[j], GRADES[j], equivalent[j], remarks[j]);
                        System.out.println("+-------------------+---------------------+-------------------------+---------------------+----------------------+-------------------+---------+");
                        }                        
                        
                    } else if (choice == 3) {
                        System.out.print("\nLOG OUT SUCCESSFULLY");
                        break;                       
                                                                   
                    } else {                                              
                        System.out.println("Choose 1, 2 or 3 only");                                                                 
                    }                                          
                
            } catch (Exception e) {        
                System.out.print("Invalid input! Enter number only! ");
                input.next();
            }               
        }
    }
} 
