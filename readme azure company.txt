Projeto Azure - Company (Relatório)

O QUE EU FIZ
-------------

1. Juntei tudo em uma linha por funcionario
   Cada linha da tabela "Funcionarios" representa UM colaborador,
   com tudo que existe sobre ele: dados pessoais, departamento,
   gerente, quantas horas trabalhou, em quantos projetos ele esta
   e quantos dependentes ele tem.

2. Arrumei os cabecalhos
   Troquei os nomes tecnicos do banco (Fname, Lname, Ssn, Dno...)
   por nomes que qualquer pessoa entende: Colaborador, Salario,
   Departamento, Gerente.

3. Separei o endereco em colunas
   O endereco vinha tudo junto em um texto so (numero, rua, cidade
   e estado misturados). Eu separei em 4 colunas: Numero, Rua,
   Cidade e Estado.

4. Tirei os nulls
   Um funcionario (o James Borg) nao tinha gerente cadastrado,
   porque ele e o presidente da empresa - nao tem ninguem acima
   dele. Em vez de deixar essa celula em branco (null), eu escrevi
   "Sem gerente (Presidencia)". Assim a tabela fica completa e sem
   nenhum campo vazio.

5. Troquei codigos por nomes
   Departamento e gerente apareciam so como numero/codigo. Eu
   troquei pelo nome de verdade (ex: em vez de "5" aparece
   "Research"; em vez do codigo do gerente aparece o nome dele).

6. Criei uma coluna para o nivel do funcionario
   Reparando na tabela, percebi que dava para descobrir quem e
   presidente, quem e gerente e quem e "time" so olhando se o nome
   da pessoa aparece na coluna Gerente de alguem. Se o proprio
   funcionario nao tem gerente, ele e presidencia. Se o nome dele
   aparece como gerente de outra pessoa, ele e gerencia. Os demais
   sao operacional. Criei a coluna Nivel_Hierarquico com essa
   logica.

7. Somei as horas trabalhadas
   Cada funcionario podia aparecer varias vezes na tabela de horas
   (uma vez para cada projeto). Eu somei tudo e coloquei em uma
   coluna so: Horas_Trabalhadas.

8. Contei os projetos e os dependentes
   Do mesmo jeito, contei em quantos projetos cada funcionario
   aparece (Qtd_Projetos) e quantos dependentes ele tem
   (Qtd_Dependentes).

9. Tirei o que nao era necessario
   Removi colunas que so serviam para o banco funcionar, mas que
   nao ajudam em um relatorio: o codigo do gerente (Super_ssn), o
   codigo do departamento (numero), e a letra do meio do nome
   (Minit). O que importa ficou; o resto saiu.



