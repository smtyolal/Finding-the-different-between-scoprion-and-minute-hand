# Finding-the-different-between-scoprion-and-minute-hand



#include <stdio.h>

double get_angle(int hour , int minute){

double angle;

angle = ( 11 * minute - 60 * hour ) / 2 ; 

if (angle < 0)
{
    angle  *= -1;
}

}


int main(){

int h, min;
printf("Please, Enter value of hour and minute in order: ");
scanf("%d%d",&h,&min);

printf("Angle is = %.2lf\n",get_angle(h,min));
    return 0;
}
