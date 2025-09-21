#include <stdio.h>


struct Carta {
    char estado;
    char codigo[4]; 
    char cidade[50];
    int populacao;
    float area;
    float PIB;
    int pontosTuristicos;
};


void lerDadosCarta(struct Carta *carta) {
    printf("--- Digite os dados da carta ---\n");
    
    
    printf("Estado (A-H): ");
    scanf(" %c", &carta->estado); 

    
    printf("Codigo da Carta (ex: A01): ");
    scanf("%s", carta->codigo);

    
    printf("Nome da Cidade: ");
    scanf(" %[^\n]", carta->cidade); 

    
    printf("Populacao: ");
    scanf("%d", &carta->populacao);

    printf("Area (em km²): ");
    scanf("%f", &carta->area);

    printf("PIB (em bilhoes de reais): ");
    scanf("%f", &carta->PIB);

    printf("Numero de Pontos Turisticos: ");
    scanf("%d", &carta->pontosTuristicos);
}


void exibirDadosCarta(struct Carta carta) {
    printf("--- Informacoes da Carta ---\n");
    printf("Estado: %c\n", carta.estado);
    printf("Codigo da Carta: %s\n", carta.codigo);
    printf("Nome da Cidade: %s\n", carta.cidade);
    printf("Populacao: %d\n", carta.populacao);
    printf("Area: %.2f km²\n", carta.area);
    printf("PIB: %.2f bilhoes de reais\n", carta.PIB);
    printf("Numero de Pontos Turisticos: %d\n", carta.pontosTuristicos);
}

int main() {
    struct Carta carta1, carta2;

    printf("--- Cadastro da Carta 1 ---\n");
    lerDadosCarta(&carta1);

    printf("\n--- Cadastro da Carta 2 ---\n");
    lerDadosCarta(&carta2);
    
    printf("\n==================================\n");
    printf("--- Cartas Cadastradas ---\n");
    
    printf("\n--- Carta 1 ---\n");
    exibirDadosCarta(carta1);

    printf("\n--- Carta 2 ---\n");
    exibirDadosCarta(carta2);

    return 0;
}
