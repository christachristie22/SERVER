Printf ( "Mo626 / Airtel money server");

#include <stdio.h>
#include <stdlib.h>
#include <math.h>

double Check_Balance();
double Send_Money();
double Top_up();
double Pay_Bills();
double Make_Payments();
double Deposit_money();

int main(){
    #define Mo626 *626#;
    #define Airtel *211#;
    int code = (626, 211);
    int pin = 1234;
    char function;
    int terminate,selected;
    int index;

    printf ("Welcome\n");

    printf("\nEnter code: ");
    scanf ("%d", &code);



    if (code = 626){

                printf("\nEnter pin: ");
                scanf("%d", &pin);

    if (pin = 1234){


    char function [20][20] ={
            "Check Balance",
            "Send Money",
            "Top Up",
            "Pay Bills",
            "Make Payments",
            "Deposit Money"
            };

    do {

              for (index = 0; index < 6; index++){


            printf("%d. %s \n", index+1, function[index]);
    }
        printf("Select option: ");
            scanf("%d", &selected);

        switch(selected){
    case 1:
        selected = Check_Balance();
        break;

    case 2:
        selected = Send_Money();
        break;

    case 3:
        selected = Top_up();
        break;

    case 4:
        selected = Pay_Bills();
        break;

    case 5:
        selected = Make_Payments();
        break;

    default:
        printf("Enter valid option\n");




    }printf ("Press 1 to continue with the program: ");
       scanf ("%d\n", &terminate); }


    while (terminate != 0);


        printf ("Thank you for Banking with us");
    }
    }

return 0;
}
double Check_Balance(){
double balance = 1000000;
int deposit_money;
int withdraw = 0;

balance = balance - withdraw;
printf("Your balance is: %.2f\n", balance);

return balance;

}
double Send_Money(){
    double amount;
    int account;
    double balance;
    int withdraw;

    printf("Enter account number: \n");
    scanf("%d", &account);

    printf("Enter amount: \n");
    scanf("%.2lf", &amount);

    if (amount < balance){
        printf("Insufficient funds\n");}

    else (amount > balance);
    balance = balance - amount;
        printf("Your transaction has been processed\n");


//    else if (amount = '0');
//        printf("Enter an amount");


return balance;
}
double Top_up(){
    double balance;
    double amount;

    printf("Enter amount: ");
    scanf("%.2lf", &amount);

    balance = balance + amount;
    printf("You have successfully topped up your account");


return balance;
}
double Pay_Bills(){
    double balance;

return balance;
}
double Make_Payments(){
    double balance;

return balance;
}
double Deposit_money(){
    double balance;

return balance;
}
