#include <stdio.h>
int main(void){
    float loan,interest_rate,payment;
    int time;
    char c[][7]={{"first"},{"second"},{"third"}};
    scanf("%f\n%f\n%f",&loan,&interest_rate,&payment);
    for(time=0; time<=2; time++){
        loan=loan*(1+interest_rate/1200)-payment;
        printf("Balance remaining after %s payment: $%.2f\n",c[time],loan);
    }
}
