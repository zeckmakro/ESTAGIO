# ESTAGIO

#include <stdio.h>

int numero(int *A, int n) {
    int i, total = 0;
    for (i = 0; i < n; i++) {
        if (A[i] == 8) {
            total += 5;
        } else if (A[i] % 2 == 0) {
            total += 1;
        } else {
            total += 3;
        }
    }
    return total;
}

int main() {
    int A[] = {1, 2, 8, 9, 8};
    int n = 5;
    int resultado = numero(A, n);
    printf("A pontuacao total sera: %d\n", resultado);
    return 0;
}
