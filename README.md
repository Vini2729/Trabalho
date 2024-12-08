# Trabalho
Sistema de Gestão de Academia:

Objetivo do Banco de Dados:
* Membros: Dados pessoais e históricos de treinamento dos alunos.
* Planos de Treinamento: Programas de treino com duração e descrição detalhada.
* Exercícios: Atividades disponíveis, incluindo tipo e descrição.
* Rotinas de Treinamento: Combinação de exercícios, séries, repetições e tempo de descanso para cada plano.
* Histórico de Treinamento: Registro de planos realizados por cada membro, incluindo status e período.

Tabelas e Relacionamentos:
Tabelas:
1. MEMBROS: Armazena informações dos membros da academia, como nome, data de nascimento, telefone e e-mail.
2. PLANOS_TREINAMENTO: Contém os planos de treinamento disponíveis, incluindo nome, descrição e duração em semanas.
3. EXERCICIOS: Lista os exercícios cadastrados, categorizados por tipo.
4. ROTINAS_TREINAMENTO: Define a relação entre planos de treinamento e exercícios, detalhando séries, repetições e tempo de descanso.
5. HISTORICO_TREINAMENTO: Registra os planos que cada membro está seguindo ou concluiu, incluindo o status e as datas de início e fim.

Relacionamentos:
* Um membro pode estar associado a vários históricos de treinamento, mas cada histórico está vinculado a um único plano.
* Um plano de treinamento pode ter várias rotinas, e cada rotina é composta por exercícios específicos.
* Um histórico de treinamento pertence a um único membro e está vinculado a um único plano.

Como Executar os Scripts:
Requisitos:
* Banco de dados Oracle instalado.
* Ferramentas como *SQL*Plus, **SQL Developer* ou qualquer outro cliente Oracle.

Scripts Disponíveis:
1. script_ddl.sql: Cria as tabelas, chaves primárias, chaves estrangeiras e restrições.
2. script_dml.sql: Insere dados representativos nas tabelas criadas.

Passos:
1. Execute o Script DDL:
   Abra o cliente Oracle de sua escolha e use o comando: @caminho_do_arquivo/script_ddl.sql
