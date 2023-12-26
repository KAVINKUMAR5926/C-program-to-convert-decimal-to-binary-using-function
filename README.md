# C-program-to-convert-decimal-to-binary-using-function
#include <stdio.h>
int dectobin(int a);
int main() {
    int a;
    scanf("%d",&a);
    dectobin(a);
    return 0;
}
int dectobin(int a){
    int arr[10],i=0,k=0;
    while(a!=0){
        int d=a%2;
        arr[i]=d;
        i++;
        a=a/2;
    }
    for(int k=i;k>=0;k--){
        printf("%d",arr[k]);
    }
}
