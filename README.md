# questao10-
10.	Seja x um vetor de 4 elementos, declarado da forma TIPO x[4]. Suponha que depois da declaração, x esteja armazenado no endereço de memória 4092 (ou seja, o endereço de x[0]). Suponha também que na máquina seja usada uma variável do tipo char ocupa 1 byte, do tipo int ocupa 2 bytes, do tipo float ocupa 4 bytes e do tipo double ocupa 8 bytes. Quais serão os valores de x+1, x+2 e x+3 se: 
◦ x for declarado como char? x=4092, x+1=4093, x+2=4094 e x+3=4095
◦ x for declarado como int? x=4092, x+1=4094, x+2=4096 e x+3=4098
◦ x for declarado como float? x=4092, x+1=4096, x+2=409A e x+3=409E
◦ x for declarado como double? x=4092, x+1=409A, x+2=40A2 e x+3=40B6
Implemente um programa de computador para testar estas suposições e compare as respostas oferecidas pelo programa com as respostas que você idealizou.

int main(){
  char x[4];
  int p;
  for(int i=0;i<4;i++){
  p = &x;
    printf("%X ",x+i); 
  }
}

#include <stdio.h>

int main(){
  int x[4];
  int p;
  for(int i=0;i<4;i++){
  p = &x;
    printf("%X ",x+i); 
  }
}

#include <stdio.h>

int main(){
  float x[4];
  int p;
  for(int i=0;i<4;i++){
  p = &x;
    printf("%X ",x+i); 
  }
}

#include <stdio.h>

int main(){
  double x[4];
  int p;
  for(int i=0;i<4;i++){
  p = &x;
    printf("%X ",x+i); 
  }
}
