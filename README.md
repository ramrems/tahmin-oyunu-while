#include<stdio.h>
#include<stdlib.h>
#include<time.h>
int main (){
int random,sayac,sayi;
srand(time(NULL));
random=rand() % 100+1;
printf("\n0 ile 100 arasinda bir sayi girerek bilgisayarin tuttugu sayiyi bulmaya calisiniz\n");
printf("ilk tahmininiz: ");
scanf("%d",&sayi);
sayac=1;
while(sayac<6 && sayi!=random){
	sayac++;
	if (sayi>random) {
printf("daha kucuk bir sayi girmeyi deneyiniz: ");}
	else{
printf("daha buyuk bir sayi girmeyi deneyiniz: ");}
	scanf("%d",&sayi);}

	if (sayi==random) {
	printf ("tebrikler dogru tahmin ettiniz");}
	else{
	printf("uzgunum tahmin hakkiniz doldu sayi %d idi",random);}

	return 0;}
