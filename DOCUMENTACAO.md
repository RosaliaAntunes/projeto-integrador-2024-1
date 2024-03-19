# Documentação

Aqui, você deve elaborar um "guia" para desenvolvedores que queiram contribuir livremente com seu projeto. Estruture este documento como achar melhor. Embora já hajam algumas seções pré-definidas, elas são apenas sugestões de qual estrutura seguir e o que escrever. 
1. Escolha uma Tarefa Antes de começar, é útil escolher uma tarefa na qual deseja trabalhar. Isso pode ser uma tarefa aberta no rastreador de problemas (issue tracker) do GitHub ou uma ideia que você tenha para melhorar o projeto.

2. Fork do Repositório Faça um fork do repositório do projeto para sua própria conta no GitHub. Isso permitirá que você faça alterações sem afetar o projeto principal.

3. Desenvolvimento da Funcionalidade ou Correção de Bugs Desenvolva a funcionalidade ou corrija o bug em sua própria branch. Certifique-se de seguir as convenções de nomenclatura de branches, como feature/nome-da-funcionalidade ou bugfix/nome-do-bug.

4. Testes Escreva testes para a nova funcionalidade ou correção de bugs, garantindo que o código funcione conforme o esperado e não introduza regressões.

5. Envio de Pull Request Quando estiver pronto, envie um pull request para o repositório principal. Certifique-se de incluir uma descrição clara das alterações realizadas e qualquer informação relevante para revisão.

6. Revisão de Código Outros membros da comunidade revisarão seu código e fornecerão feedback. Esteja aberto a sugestões e modificações para melhorar a qualidade do código.

7. Fusão do Pull Request Após a revisão e aprovação, seu pull request será mesclado (merged) ao repositório principal.


## Instruções de deploy

Faça uma pequena pesquisa sobre como fazer o [*deploy*](https://en.wikipedia.org/wiki/Software_deployment) de um projeto web com Python e Django e escreva aqui algumas orientações breves.  Fazer o *deploy* não é obrigatório para a avaliação, mas é importante que os desenvolvedores do projeto tenham ao menos uma noção de como isso é feito.

Sugestões de serviços de hospedagem para pesquisar:
* Vercell
* PythonAnywhere
* AWS Elastic Beanstalk (não recomendamos o uso deste serviço sem supervisão, pois pode gerar cobranças inesperadas)

## Modelagem de banco de dados

id: Este é um campo automaticamente gerado pelo Django para servir como chave primária da tabela.
nome: Um campo do tipo CharField que armazena o nome da matéria.
primeira_nota, segunda_nota, terceira_nota, quarta_nota: Campos do tipo IntegerField que armazenam as notas dos quatro bimestres.
media_notas: Um campo do tipo IntegerField que armazena a média das notas, calculada automaticamente no momento em que o objeto é salvo.
Portanto, a modelagem resultante no banco de dados seria algo semelhante a isso:


| id |    nome    | primeira_nota | segunda_nota | terceira_nota | quarta_nota | media_notas |
|----|------------|---------------|--------------|---------------|-------------|-------------|
|  1 | Matemática |            80 |           75 |            85 |          90 |          82 |
|  2 | Português  |            70 |           85 |            90 |          80 |        81.25|
| .. | .......... | ............. | ............ | ..............| ........... | ........... |

Cada linha representa um registro na tabela nota_nota (supondo que nota seja o nome do aplicativo onde está definido o modelo Nota). A coluna media_notas é calculada automaticamente pelo método save definido no modelo Nota.





