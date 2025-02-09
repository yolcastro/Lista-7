#include <stdio.h>

struct PROFESSOR {
    char nome[100];
    char sobrenome [100];
};

struct DISCIPLINA {
    char nome[100];
    int cargaHoraria;
    struct PROFESSOR professor;
};

void dadosProfessor(struct PROFESSOR* professor) {
    printf("Professor: %s %s\n", professor -> nome, professor -> sobrenome);
}

void dadosDisciplina(struct DISCIPLINA* disciplina) {
    printf("Disciplina: %s\n", disciplina -> nome);
    printf("Carga horária: %d horas\n", disciplina -> cargaHoraria);
    dadosProfessor(&disciplina -> professor);
}

int main() {
    struct DISCIPLINA disciplina;
    
    printf("Preencha as informações abaixo:\n");

    printf("Nome da disciplina:\n");
    fgets(disciplina.nome, 50, stdin);
    disciplina.nome[strcspn(disciplina.nome, "\n")] = '\0';
    
    printf("Carga horária da disciplina:\n");
    scanf("%d", &disciplina.cargaHoraria);

    printf("Nome do professor:\n");
    getchar();
    fgets(disciplina.professor.nome, 50, stdin);
    disciplina.professor.nome[strcspn(disciplina.professor.nome, "\n")] = '\0';

    printf("Sobrenome do professor: ");
    fgets(disciplina.professor.sobrenome, 50, stdin);
    disciplina.professor.sobrenome[strcspn(disciplina.professor.sobrenome, "\n")] = '\0';

    printf("Dados sobre a disciplina:\n");
    dadosDisciplina(&disciplina);

    return 0;
}
