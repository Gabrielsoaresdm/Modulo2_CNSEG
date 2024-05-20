# Módulo 2 – Sistema RESILIADATA
## Objetivo
O objetivo do projeto é realizar a modelagem (conceitaul e lógico) de um banco de dados da empresa Resilia. 

A Atividade consistem em 4 perguntas sendo:
```
1 - Quais são as entidades necessárias?
```
Empresa_Parceira: Representa as empresas parceiras.

Tecnologia: Representa as tecnologias disponíveis.

Colaboradores: Representa os colaboradores que trabalham para as empresas parceiras.

```
2 - Quais são os principais campos e seus respectivos tipos?
```
## Principais Campos e Tipos de Dados:

Empresa_Parceira:
id_empresa (INT): Chave primária autoincrementada.

nome (VARCHAR): Nome da empresa.

email (VARCHAR): Endereço de e-mail da empresa.

localização (VARCHAR): localização da empresa.

Tecnologia:
id_tecnologia (INT): Chave primária autoincrementada.

nome (VARCHAR): Nome da tecnologia.

area (VARCHAR): Área de aplicação da tecnologia.

Colaboradores:
id_colaborador (INT): Chave primária autoincrementada.

nome (VARCHAR): Nome do colaborador.

idade (VARCHAR): idade do colaborador.

id_empresa (INT): Chave estrangeira referenciando a tabela Empresa_Parceira.


3 - Relacionamentos entre as Entidades:
```
Empresa_Parceira e Colaboradores: Relacionamento de 0 para N, indicando que uma empresa pode ter vários colaboradores e os colaboradores podem trabalhar para n empresas.

Empresa_Parceira e Tecnologia_Utilizada: Relacionamento de 1 para N, indicando que uma empresa pode utilizar várias tecnologias e uma tecnologia pode ser utilizada por várias empresas.

4 - Simule 2 registros para cada entidade.
```
## Adicionar registros para Empresa_Parceira

INSERT INTO Empresa_Parceira (nome, email, localização) VALUES 
('Empresa A', 'empresa_a@example.com', 'Rua exemplo'),
('Empresa B', 'empresa_b@example.com', 'Rua exemplo');

Adicionar registros para Tecnologia
INSERT INTO Tecnologia (nome, area) VALUES 
('Java', 'Desenvolvimento de software'),
('Python', 'Ciência de dados');

Adicionar registros para Colaborador
INSERT INTO Colaborador (nome, idade, cargo, id_empresa) VALUES 
('João', '27 anos', 'Desenvolvedor'),
('Maria', '29 anos', 'Analista de Dados');
