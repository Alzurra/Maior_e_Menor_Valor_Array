# Maior_e_Menor_Valor_Array
#include <iostream>
#include <time.h>
#include <locale.h>

using namespace std;

int main()
{
    
    int v[10];
    int maior,menor;
    
    setlocale(LC_ALL,"portuguese");
    
    cout<<"Vetor v[i]"<<endl;
    srand(time(NULL));
    for(int i=0;i<10;i++){
        v[i]=rand()%11;
        cout<<"["<<v[i]<<"]"<<" ";
        if(i==0){
            maior = menor = v[i];
        }else if(v[i]>maior){
            maior = v[i];
        }else if(v[i]<menor){
            menor = v[i];
        }
    }
    cout<<endl;
    cout<<"O maior valor dentro do array é o número: "<<maior<<endl;
    cout<<"O menor valor dentro do array é o número: "<<menor<<endl;
    return 0;
}
