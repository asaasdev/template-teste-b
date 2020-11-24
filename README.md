<!-- ABOUT THE PROJECT -->
## Introdução

Este teste é parte do processo seletivo aqui no Asaas para posições na Engenharia. Você precisará construir uma aplicação simples, utilizando a tecnologia ou framework com o qual se sente mais confortável, respeitando as regras de negócio propostas logo abaixo.

Caso não consiga implementar alguma das regras propostas, não se preocupe, você pode compensar menos funcionalidades garantindo que o código das que forem implementadas esteja muito bem feito.

## O que vamos avaliar

Nossa intenção com este teste é avaliar sua habilidade de constuir uma aplicação simples aplicando as melhores práticas de desenvolvimento.

Ao revisar seu código vamos avaliar os seguintes pontos:
* Organização do código.
* Respeito as regras de negócio.
* Código bem escrito, limpo e coeso.
* Uso correto do versionamento do git.
* Documentação com instruções claras e objetivos para rodar o projeto (README.md).

## O que deve ser implementado
O sistema proposto consiste em um cadastro simples com algumas regras de negócio:

1. Deve ser possível incluir, editar, remover e listar cobranças.
2. As informações contidas em uma cobrança são: nome, e-mail e CPF do cliente, data de vencimento, valor, forma de pagamento (Boleto Bancário ou Cartão de Crédito), status (Pendente, Paga ou Vencida), data de pagamento e descrição. Destas informações, são obrigatórias nome do cliente, CPF, valor, forma de pagamento e data de vencimento.
3. Considera-se removida a cobrança cujo atributo deleted seja igual a true, ou seja, ao remover uma cobrança o registro não deve ser apagado do banco, somente marcado como deletado. Uma vez removida, a cobrança não deve mais ser listada.
4. Criar uma funcionalidade que permita marcar uma cobrança como paga e não permitir qualquer alteração ou remoção uma vez que isso tenha sido feito.
5. Não permitir inserir uma cobrança com vencimento inferior à data de hoje.
6. Não permitir CPF ou email de cliente inválidos.
7. Criar um job que roda de segunda a sexta, às 8hrs. Esse job deve mudar o status de todas as cobranças pendentes que vencem antes da data atual para vencido.
8. A interface da aplicação deve ser em português.
9. Incluir os seguintes filtros na listagem: nome ou e-mail do cliente em campo único, data de vencimento inicial e final, forma de pagamento e status. Esta listagem deve ser paginada.
10. O código fonte deve ser escrito em inglês.

## Enviando o projeto
1. Apague o conteúdo deste arquivo e adicione as informações que julgar necessário, por exemplo, como rodar o projeto.
2. Abra um PR apontando para a branch `main` deste repositório.
3. Na descrição do PR, escreva o que achar relevante para quem for revisar seu código.
