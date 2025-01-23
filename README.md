# Projeto de Dados de Tutores e Alunos

Este projeto contém dois conjuntos de dados: **Tutores** e **Alunos**, ambos com características específicas para auxiliar na criação de uma plataforma de reforço escolar. O objetivo é fornecer informações sobre tutores qualificados e alunos que buscam apoio educacional.

## Características dos Bancos de Dados

### 1. **Banco de Dados de Tutores**
O banco de dados de **Tutores** contém informações sobre professores qualificados, suas áreas de ensino e detalhes de contato. Cada tutor pode ensinar uma ou mais disciplinas e tem um preço por hora determinado.

#### Características:
- **id_tutor**: Identificador único para cada tutor.
- **nome**: Nome completo do tutor.
- **nivel_escolaridade_adotado**: Nível de escolaridade (Ensino Fundamental ou Ensino Médio).
- **nivel_graduacao**: Nível de formação do tutor (Graduação, Mestrado ou Doutorado).
- **formacao**: Área de formação (ex: Matemática, História, Geografia, etc).
- **disciplinas_ensino**: Lista das disciplinas que o tutor ensina, podendo incluir múltiplas disciplinas relacionadas (ex: "Matemática, Física").
- **preco_por_hora**: Valor cobrado por hora de aula.
- **cep**: CEP (Código de Endereçamento Postal) do local de residência do tutor.

#### Exemplo de Tutor:
```csv
id_tutor,nome,nivel_escolaridade_adotado,nivel_graduacao,formacao,disciplinas_ensino,preco_por_hora,cep
1,"Eduarda Gomes","Ensino Médio","Graduação","Matemática","Matemática, Física",75.50,"58000-000"
2,"Felipe Pereira","Ensino Fundamental","Mestrado","História","História, Geografia",60.00,"58400-000"


### 2. **Banco de Dados de Alunos**
O banco de dados de **Alunos** contém informações sobre os estudantes, suas dificuldades acadêmicas e o tipo de apoio educacional que eles buscam. O objetivo é fornecer um perfil detalhado para que os tutores possam oferecer o melhor suporte possível.

#### Características:
- **id_aluno**: Identificador único para cada aluno.
- **nome**: Nome completo do aluno.
- **idade**: Idade do aluno.
- **serie_escolar**: Série escolar em que o aluno está matriculado (ex: 5º ano, 6º ano, Ensino Médio).
- **dificuldades**: Disciplinas nas quais o aluno tem maior dificuldade (ex: Matemática, Português).
- **tipo_aula**: Tipo de aula que o aluno busca (ex: "Acompanhamento", "Focado em Provas").
- **cep**: CEP do local onde o aluno reside.
- **complemento_dificuldade**: Caso o aluno tenha necessidades educacionais especiais, como "TDAH", "Espectro Autista", ou "Dislexia".

#### Exemplo de Aluno:
```csv
id_aluno,nome,idade,serie_escolar,dificuldades,tipo_aula,cep,complemento_dificuldade
1,"João Silva",14,"8º ano","Matemática","Acompanhamento","58000-001","TDAH"
2,"Maria Souza",17,"Ensino Médio","Português, Redação","Focado em Provas","58400-001","Dislexia"
