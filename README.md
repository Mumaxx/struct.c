#include<stdio.h>
#include<stdlib.h>
struct tp_endereco{
	char rua[40];
	int numero;
	char bairro[40];
	char cidade[40];
	int cep;
};

struct tp_data_nascimento{
	int dia;
	int idade;
	int mes;
};

struct cadastro_cliente{
	char nome_cliente[40];
	int telefone;
	
	struct tp_enderco  endereco;
	struct tp_data_nascimento  data_nascimento;
	};
cad_cliente[2];

int main(void){
	
	int i;
	
	printf("\n\n----CADASTRO CLIENTE----\n\n");
	
	for(i=0; i<2; i++){
		printf("\n\nNome cliente...:");
		fflush(stdin);
		gets(cad_cliente[i].nome_cliente);
		
		printf("\n\nTelefone Cliente...:");
		scanf("%d", &cad_cliente[i].telefone);
		
		printf("\n\nRua...:");
		fflush(stdin);
		gets(cad_cliente[i].endereco.rua);
		
			printf("\n\nBairro...:");
		fflush(stdin);
		gets(cad_cliente[i].endereco.bairro);
		
			printf("\n\nCidade...:");
		fflush(stdin);
		gets(cad_cliente[i].endereco.cidade);
		
		printf("\n\nNumero...:");
		scanf("%d", &cad_cliente[i].endereco.numero);
		
		printf("\n\nCep...:");
		scanf("%d", &cad_cliente[i].endereco.cep);
		
		
		printf("\n\n Dia  nasc...:");
		scanf("%d", &cad_cliente[i].data_nascimento.dia);
		
		printf("\n\n Mes nasc...:");
		scanf("%d", &cad_cliente[i].data_nascimento.mes);
		
		printf("\n\n Ano nasc...:");
		scanf("%d", &cad_cliente[i].data_nascimento.ano);
	}
	
	
	system("pause");
	return 0;

}
