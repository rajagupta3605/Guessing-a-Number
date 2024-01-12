# Guessing-a-Number
#include<stdio.h>
#include<stdlib.h>
#include<time.h>
int main(){
	int num,guess,nguess=1;
	srand(time(0));
	num=rand()%100;
//	printf("The number is %d",num);
	do{printf("Guess the number between 1 to 100\n");
	scanf("%d",&guess);
	if(guess>num){
		printf("Lower number please\n");
	}
	else if(guess<num)
	{printf("Higher number please\n");}
	else 
	{printf("You guessed number is in %d attempt\n",nguess);
	}nguess++;
	}while(guess!=num);
	
	return 0;
}


