#include <stdio.h>

// Definição da struct Aluno
typedef struct {
    char nome[50];
    char RA[15];
    float notas[5];
} Aluno;


// Função para cadastrar o aluno
void cadastrarAluno(Aluno *aluno) {

    printf("================ CADASTRAR ALUNO ==================\n");

    printf("Nome: ");
    scanf(" %49[^\n]", aluno->nome);

    printf("RA: ");
    scanf("%14s", aluno->RA);

    // Cadastro das 5 notas
    for (int i = 0; i < 5; i++) {
        printf("Nota %d: ", i + 1);
        scanf("%f", &aluno->notas[i]);
    }
}


// Função para calcular a média
float calcularMedia(Aluno aluno) {

    float soma = 0;

    for (int i = 0; i < 5; i++) {
        soma += aluno.notas[i];
    }

    return soma / 5;
}


// Função para mostrar o RA
void mostrarRA(Aluno aluno) {

    printf("RA: %s\n", aluno.RA);
}


int main() {

    Aluno aluno1;
    float media;

    // Cadastro
    cadastrarAluno(&aluno1);

    // Calcula a média
    media = calcularMedia(aluno1);

    // Exibe os dados
    printf("\n======= DADOS DO ALUNO ==========\n");

    printf("Nome: %s\n", aluno1.nome);

    mostrarRA(aluno1);

    printf("Notas:\n");

    for (int i = 0; i < 5; i++) {
        printf("Nota %d: %.1f\n", i + 1, aluno1.notas[i]);
    }

    printf("Media: %.1f\n", media);

    return 0;
}
