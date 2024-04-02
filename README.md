# Banco de Dados Escolar
Este banco de dados escolar é projetado para gerenciar informações sobre cursos, alunos, professores, matérias e matrículas. Ele foi desenvolvido usando SQL e contém uma série de comandos para criação das tabelas, inserção de dados e consultas.

## Remoção de Tabelas
Para começar, o script SQL remove todas as tabelas existentes no banco de dados, incluindo "Matricula", "Aluno", "Materia", "Professor" e "Curso". Isso é feito usando o comando DROP TABLE IF EXISTS, que garante que as tabelas sejam removidas apenas se existirem.

## Criação das Tabelas
Em seguida, o script cria as tabelas necessárias para o funcionamento do banco de dados:

- Curso: Armazena informações sobre os cursos oferecidos, com uma chave primária CursoID e o nome do curso.
- Aluno: Contém detalhes sobre os alunos matriculados, incluindo uma chave primária AlunoID, nome do aluno, RA e uma chave estrangeira CursoID que referencia o curso ao qual o aluno está associado.
- Professor: Registra informações sobre os professores, com uma chave primária ProfessorID, RP e nome do professor.
- Materia: Armazena dados sobre as disciplinas oferecidas, com uma chave primária MateriaID, nome da matéria, CursoID (chave estrangeira que referencia o curso ao qual a matéria está associada) e ProfessorID (chave estrangeira que referencia o professor responsável pela matéria).
- Matricula: Esta tabela associa alunos a matérias nas quais estão matriculados, utilizando uma chave primária composta pelas chaves estrangeiras AlunoID e MateriaID.

## Inserção de Dados
Após a criação das tabelas, o script insere dados de exemplo em algumas delas. São inseridos registros nas tabelas "Curso", "Aluno", "Professor", "Materia" e "Matricula" para simular um ambiente acadêmico.

## Consultas :
O script também inclui consultas SQL para extrair informações úteis do banco de dados, como:

- Encontrar os professores de um aluno específico.
- Identificar as matérias com mais de 3 alunos matriculados.
- Listar os alunos de um determinado professor, evitando repetições de nomes.
- Contar o número total de professores e alunos matriculados.
- Encontrar matéria sem professor.

### Autor
Este banco de dados foi criado por JuliaDuran15.
