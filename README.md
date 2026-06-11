# ✈️ Sistema para Agência de Viagens - uc 06 SENAC

Este projeto consiste no desenvolvimento do módulo backend (em formato console) de um sistema para uma agência de viagens, aplicando os conceitos fundamentais da **Programação Orientada a Objetos (POO)** em Java.

Resultado: Nota Máxima (A) obtida nesta atividade prática.

## Contexto do Projeto
A proposta deste sistema é gerenciar o registro de pacotes de viagens e o controle de dados de vendas. 
* Um Pacote de Viagem é composto por um meio de transporte e uma hospedagem, além de um destino e quantidade de dias.
* A Venda consolida os dados do cliente, a forma de pagamento e o pacote adquirido, sendo capaz de lidar com conversões de moedas (Dólar para Real).

## Regras de Negócio e Funcionalidades Implementadas

O sistema foi estruturado através das seguintes classes e responsabilidades:

1. **`Transporte`**: Armazena o tipo de transporte (aéreo, rodoviário, marítimo, etc.) e seu respectivo valor.
2. **`Hospedagem`**: Registra a descrição e o valor da diária.
3. **`PacoteViagem`**: 
   * Calcula o total da hospedagem baseado na quantidade de dias.
   * Aplica a margem de lucro (porcentagem) sobre os custos.
   * Calcula o valor total do pacote em **Dólar ($)**, somando transporte, hospedagem, margem de lucro e taxas adicionais.
4. **`Venda`**: 
   * Registra os dados do cliente e a forma de pagamento.
   * Realiza a conversão monetária de valores em Dólar para Real (R$) com base na cotação informada pelo usuário.
   * Exibe o resumo financeiro da venda nas duas moedas.
5. **`Classe Principal (Main)`**: Gerencia a interação em modo console, permitindo a entrada de dados pelo usuário, o cadastro completo da venda e a exibição organizada do relatório final.


## 💻 Conceitos Praticados
* Encapsulamento e visibilidade de atributos
* Métodos construtores para inicialização de objetos
* Lógica matemática aplicada (cálculos de porcentagem, acréscimos e conversão cambial)
* Interação com o usuário via console em Java
