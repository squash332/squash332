    #include <stdio.h>
    int main()
    }
    float a[13][13];
    int i,j;
    int n;
    int min[0][0];
    
    do { 
        printf("unesite dimenzije kvadratne matrice:");
        scanf("%d", &n);
    }
    while(n<3 || n>13);
    
    for(i=0; i<n; i++) {
        for(j=0; j<n; j++) {
            scanf("%f", &a[i][j]);
        }
    }
    for(i=0; i<n; i++) {
        for(j=0; j<n; j++){
            if(i+j>n-1) {
                if(a[i][j]>0) {
                    printf("\n%f", a[i][j]);
                }
            }
            else if(i<j) {
                if(a[i][j]>0) {
                    printf("\n%f", a[i][j]);
                }
            }
            }
    }
    return 0;
    }
