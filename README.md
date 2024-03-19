<!-- Adicione Badges das tecnologias que você usou aqui -->
<!-- Você pode encontrar badges aqui: https://github.com/Ileriayo/markdown-badges?tab=readme-ov-file#markdown-badges -->
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white)
![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)

**Este projeto foi desenvolvido como atividade final do curso de capacitação em Python da Cyber Edux, realizado de setembro de 2023 até março de 2024. Para mais informações, consulte o [enunciado](ENUNCIADO.md).**

# Sistema de notas

<!-- Substitua a seguinte imagem por uma logo do seu projeto -->
<img src="https://i.pinimg.com/736x/e6/7e/2b/e67e2b08be77df9a22c7caf517989b5f.jpg" width="150px">

<!-- Substitua o seguinte parágrafo por um resumo do seu projeto: -->

**Definição dos Requisitos:**
Antes de começar a codificar, passei um tempo detalhando os requisitos do sistema. Identifiquei os diferentes tipos de usuários - alunos, professores e administradores - e as funcionalidades essenciais, como inserção de notas, visualização de desempenho dos alunos e gerenciamento de turmas.

**Modelagem de Dados:**
Com os requisitos em mãos, comecei a projetar o banco de dados do sistema. Criei modelos Django para representar entidades como alunos, professores, disciplinas, turmas e notas. Por exemplo, o modelo de aluno contém campos como nome, idade e turma, enquanto o modelo de nota registra a pontuação de um aluno em uma disciplina específica.

**Implementação das Views e Templates:**
A próxima etapa foi criar as views e templates para a interface do usuário. Usei as views do Django para processar solicitações HTTP e renderizar templates HTML. Desenvolvi páginas web para funcionalidades como inserção de notas, visualização de desempenho dos alunos e geração de relatórios.

**Autenticação e Autorização:**
Garantir a segurança do sistema foi uma prioridade. Implementei a autenticação e autorização do Django para controlar o acesso dos usuários às diferentes partes do sistema. Isso garante que apenas usuários autorizados possam visualizar ou modificar dados sensíveis.

**Implementação de Funcionalidades Específicas:**
Com a estrutura básica em funcionamento, concentrei-me em implementar funcionalidades específicas, como a capacidade dos professores de inserir notas e os alunos de visualizar seus próprios resultados. Isso envolveu escrever lógica personalizada e integrar bibliotecas Python para realizar cálculos e manipulações de dados.

**Testes:**
Testar o sistema foi uma etapa crucial. Usei as ferramentas de teste do Django para escrever testes automatizados que garantem o bom funcionamento do sistema e evitam regressões. Testei cada funcionalidade para garantir que ela funcionasse conforme o esperado.

**Implantação:**
Por fim, implantei o sistema em um servidor web para que pudesse ser acessado pelos usuários finais. Optei por hospedá-lo em um serviço de nuvem para garantir escalabilidade e confiabilidade.



## Documentação

* [Documentação (para desenvolvedores)](DOCUMENTACAO.md)
* [Manual (para usuários)](MANUAL.md)

## Sobre o autor

<!-- Coloque seu nome, uma foto sua e uma pequena bio sobre você na seguinte tabela: -->
|  |  |
|:-------------:|:------------------------------------------------------------:|
|  <img src="https://i.pinimg.com/564x/01/49/c6/0149c6136b1b567d188241d77990719f.jpg" width="150px"></br> **Rafaela Fernandes De Sousa Ribeiro Leite** | Meu nome é Rafaela Fernandes de Sousa Ribeiro Leite, tenho 20 anos e sou natural de Mato Grosso, Brasil. Desde sempre, tive um interesse profundo tanto pela educação quanto pela tecnologia, e é isso que tem moldado minha jornada até aqui. Atualmente, estou cursando Pedagogia na Universidade Federal de Mato Grosso. Escolhi esse caminho porque acredito que a educação é uma ferramenta poderosa para transformar vidas e comunidades. Quero contribuir para a melhoria do sistema educacional brasileiro e ajudar a proporcionar uma educação de qualidade para todos.Além dos meus estudos em Pedagogia, também estou fazendo um curso técnico de Python. Sempre fui fascinada pela tecnologia e suas possibilidades, e aprender uma linguagem de programação como Python me permite explorar novas maneiras de usar a tecnologia para o bem da sociedade. Estou animada para ver como posso integrar meus conhecimentos em pedagogia e tecnologia para criar soluções inovadoras que beneficiem a educação e a sociedade como um todo.|
