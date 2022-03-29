# Testes automatizados com JUnit

Este projeto foi gerado para simular  um controle de funcionários, reajustes salariais e cálculo de bônus. Nele, iniciamos com duas classes: 
Funcionário e BonusService. A primeira (Funcionario) representa um funcionário dentro de uma empresa, reunindo dados como nome, data de admissão (dataAdmissao) 
e salário (salario). Além de ter um constructor para receber essas três informações e alguns métodos gets para recuperá-las. A segunda (BonusService) é uma classe de serviço 
que executa uma regra de negócio da aplicação, que é a de calcular o bônus a ser recebido por um funcionário.
Vamos começar testando o cenário em que o salário do funcionário é muito alto e o seu bônus ultrapassa mil reais. Conforme a classe BonusService, 
essa pessoa não tem direito a bônus.

É aqui que entra o **JUnit**, que se tornou a biblioteca padrão por ser amplamente utilizada para a escrita de testes automatizados em linguagem Java.

O **JUnit** é uma biblioteca gratuita e de código aberto. Seu código-fonte pode ser encontrado em <https://github.com/junit-team/junit5>. Sua função principal é 
simplificar a escrita de testes de unidade (ou testes unitários), que são a categoria mais simples dos testes automatizados.

---

# TDD (Test Driven Development)

**TDD (do inglês Test Driven Development), ou seja, Desenvolvimento Guiado pelo Teste**. Nesta abordagem começamos escrevendo o teste automatizado para depois implementar o código.
No **TDD**, escrevemos o teste, implementamos o mínimo necessário para ele funcionar corretamente num determinado cenário e passamos por uma terceira etapa que é a refatoração (ou refactoring), 
prática usada para melhorar um código existente.

Para implementar essa funcionalidade em nosso projeto criamos uma classe de teste referente ao reajuste anual de salário dos funcionários de uma empresa.
O sistema deve permitir que os funcionários recebam um reajuste salarial anual baseado em seu desempenho, obedecendo às seguintes regras:

- Se o desempenho for classificado como "A desejar", o reajuste será de 3% do salário atual.
- Se o desempenho for "Bom,", o reajuste será de 15% do salário.
- Se o desempenho for "Ótimo", o reajuste será de 20% do salário.

---

# Refactoring (Refatoração)

Qual o papel da refatoração no TDD?

A **refatoração** de software tem como finalidade aumentar a qualidade do projeto em relação aos atributos de reusabilidade, manutenibilidade e legibilidade. 
Um aspecto importante de uma **refatoração** é que ela melhora o software sem mudar o comportamento do mesmo; uma **refatoração** não adiciona nem remove funcionalidades.

