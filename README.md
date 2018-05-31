# Jogo




#include <stdio.h>
#include <stdlib.h>
#include <unistd.h>


void player1(){
printf("Player 1\n");
}

void player2(){
printf("Player 2\n");
}

char tabuleiro(){

char tabuleiro[10][10]={	{'1', '*', '*', '*', '*', '*', '*', '*', '*', '2',},
   							{'*', '*', '*', '*', '*', '*', '*', '*', '*', '*',},
   							{'*', '*', '*', '*', '*', '*', '*', '*', '*', '*',},
   							{'*', '*', '*', '*', '*', '*', '*', '*', '*', '*',},
							{'*', '*', '*', '*', '*', '*', '*', '*', '*', '*',},
   							{'*', '*', '*', '*', '*', '*', '*', '*', '*', '*',},
  							{'*', '*', '*', '*', '*', '*', '*', '*', '*', '*',},
  							{'*', '*', '*', '*', '*', '*', '*', '*', '*', '*',},
   							{'*', '*', '*', '*', '*', '*', '*', '*', '*', '*',},
   							{'*', '*', '*', '*', '*', '*', '*', '*', '*', '*' }};
int L=0,C=0;

	do{
		do{ 
		printf("%c",tabuleiro[L][C]);
		C++;
		}while(C<10);
	C= 0;

	L++;
	}while(L<10);
return 0;
}

continuar(){
int unic;
printf("Gostaria de Jogar Novamente?\n1\tSim\n2\tNao\n");
scanf("%d",&unic);
	while(unic!=1 && unic!=2){
	printf("Por favor, digite um valor valido\n1\tSim\n2\tNao\n");
	scanf("%d",&unic);
	}
		if (unic==1)
		
			else if(unic==2)
			return 0;
}




int main(){

printf("Bem vindo ao joguinho, o programa vai escolher aleatoriamente quem inicia e eh nois");
tabuleiro();
sleep(5);
system("cls");
int unic=rand()%2==0;
	if (unic==0)
	player1();
		else
		player2();
continuar();
}
