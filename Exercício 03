#include <stdio.h>
#include <stdlib.h>
#include <time.h>

#define MX 100

struct INFORMACOES {
    int *vetor;
    int tamanho;
    double media;
};

int *alocarMemoria(int n) {
    int *p = NULL;

    if (!(p = (int*) malloc(n * sizeof(int)))) {
        puts("Memória insuficiente");
        exit(1);
    }

    return p;
}

void preencherVetor(int *p, int n) {
    for (int k = 0; k < n; k++) {
        *(p + k) = rand() % MX;
    }
}

void imprimirVetor(int *p, int n) {
    for (int k = 0; k < n; k++) {
        printf("[%p] %d\n", p + k, *(p + k));
    }
}

double calcularMedia(int *p, int n) {
    int soma = 0;
    for (int k = 0; k < n; k++) {
        soma += *(p + k);
    }
    return (double) soma / n;
}

int main() {
    struct INFORMACOES info;
    int tam;

    srand(time(NULL));

    printf("Digite o tamanho desejado do vetor: ");
    scanf("%d", &tam);

    info.tamanho = tam;
    info.vetor = alocarMemoria(tam);
    
    preencherVetor(info.vetor, tam);
    info.media = calcularMedia(info.vetor, tam);

    printf("Vetor:\n");
    imprimirVetor(info.vetor, tam);
    
    printf("Média dos valores: %.2f\n", info.media);

    free(info.vetor);

    return 0;
}
