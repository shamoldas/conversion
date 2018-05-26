#include<stdio.h>
main(){

    float km, m, cm, mm;
    int condition;

    do{

        do{
            printf("Press 1 for conversion from km to others\n");
            printf("Press 2 for conversion from m to others\n");
            printf("Press 3 for conversion from cm to others\n");
            printf("Press 4 for conversion from mm to others\n");
            printf("Enter 0 for exit \n");

            scanf("%d",&condition);

            if(condition>4 || condition <0){
                printf("YOU CAN PRESS ONLY 0 TO 4 FOR WORK THE PROGRAM\n");
                printf("Try Again\n\n");
            }
        }while(condition>4 || condition <0);



    if(condition == 1){
        printf("Enter value in KM : ");
        scanf("%f",&km);

        m = km*1000;
        cm = m*100;
        mm = cm*10;

        printf("%f km is equal = %f meter\n",km,m);
        printf("%f km is equal = %f centi-meter\n",km,cm);
        printf("%f km is equal = %f mili-meter\n",km,mm);
    }

    if(condition == 2){
        printf("Enter value in M unit: ");
        scanf("%f",&m);

        km = m/1000;
        cm = m*100;
        mm = cm*10;

        printf("%f m is equal = %f kilo meter\n",m,km);
        printf("%f m is equal = %f centi-meter\n",m,cm);
        printf("%f m is equal = %f mili-meter\n",m,mm);
    }

    if(condition == 3){
        printf("Enter value in CM unit: ");
        scanf("%f",&cm);

        m = cm/100;
        km = m/1000;
        mm = cm*10;

        printf("%f cm is equal = %f kilo meter\n",cm,km);
        printf("%f cm is equal = %f mili-meter\n",cm,mm);
        printf("%f cm is equal = %f meter\n",cm,m);
    }

    if(condition == 4){
        printf("Enter value in MM unit: ");
        scanf("%f",&mm);

        cm = mm/10;
        m = cm/100;
        km = m/1000;

        printf("%f mm is equal = %f meter\n",mm,m);
        printf("%f mm is equal = %f centi-meter\n",mm,cm);
        printf("%f mm is equal = %f kilo-meter\n",mm,km);
    }

    printf("\n\n");
    }while(condition != 0);

}

