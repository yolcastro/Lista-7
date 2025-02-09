#include <stdio.h>

struct ALUNO {
    float n1;
    float n2;
    float media;
};

void calcular_media(struct ALUNO* aluno) {
    aluno -> media = (aluno -> n1 + aluno -> n2) / 2;
}

int main() {
    struct ALUNO alunos[3];
    
    for (int i = 0; i < 3; i++) {
        printf("Digite a primeira nota do aluno %d: ", i + 1);
        scanf("%f", &alunos[i].n1);
        printf("Digite a segunda nota do aluno %d: ", i + 1);
        scanf("%f", &alunos[i].n2);

        calcular_media(&alunos[i]);
    }

    for (int i = 0; i < 3; i++) {
        printf("Aluno %d\n", i + 1);
        printf("Nota 1: %.2f\n", alunos[i].n1);
        printf("Nota 2: %.2f\n", alunos[i].n2);
        printf("Média: %.2f\n", alunos[i].media);
    }

    return 0;
}
