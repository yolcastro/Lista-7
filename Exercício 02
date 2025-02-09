#include <stdio.h>
#include <stdlib.h>
#include <string.h>

#define TAM 100

struct ESTOQUE {
    char nomePeca[TAM];
    int numPeca;
    float valorPeca;
    int numPedido;
};

int main() {
    struct ESTOQUE estoque;

    printf("Preencha as informações abaixo sobre o pedido:\n");
    printf("Nome da peça: ");
    fgets(estoque.nomePeca, sizeof(estoque.nomePeca), stdin);

    printf("Número da peça: ");
    scanf("%d", &estoque.numPeca);

    printf("Valor da peça: ");
    scanf("%f", &estoque.valorPeca);

    printf("Número do pedido: ");
    scanf("%d", &estoque.numPedido);

    printf("\nInformações cadastradas do pedido:\n");
    printf("Nome da peça: %s", estoque.nomePeca);
    printf("Número da peça: %d\n", estoque.numPeca);
    printf("Valor da peça: %.2f\n", estoque.valorPeca);
    printf("Número do pedido: %d\n", estoque.numPedido);

    return 0;
}
