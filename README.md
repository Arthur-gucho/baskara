// entrada:a,b,c
// saida:x' e x''
//processamento:calculo
#include<stdio.h>// biblioteca para entrada e saida de dados printf e scanf
#include<math.h>// biblioteca para funçoes matematicas 
int main(){//inicio do algoritmo funçao:main
double a, b, c, x1, x2, delta;
printf("digite o valor de a:");//exibe mensagem na tela
scanf("%lf",&a);
printf("digite o valor de b:");
scanf("%lf",&b);
printf("digite o valor de c:");
scanf("%lf",&c);
//x1=(-(b)+sqrt(b*b-4*a*c))(/2*a)
//condiçao,nao se pode dividir por zero
if(a==0||delta<0)//==(igual) !=(diferente) <(menor que) >(maior que) <=(menor ou igual) >=(maior ou igual)
{
printf("impossivel calcular!\n");
}
else//senao
{
	delta=pow(b,2)-4*a*c;
	x1=(-(b)+sqrt(delta))/(2*a);
	x2=(-(b)-sqrt(delta))/(2*a);
	printf("x1=%.2lf\tx2=%.4lf\n",x1,x2);
	return 0;}
}
