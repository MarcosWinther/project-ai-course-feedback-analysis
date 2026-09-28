# 🎓 AI Course Feedback Analysis

Projeto de análise de feedbacks de alunos utilizando Inteligência Artificial para identificar padrões, sentimentos, problemas recorrentes e oportunidades de melhoria em cursos online.

<br>

## 📌 Sobre o projeto

Este projeto foi desenvolvido como um desafio prático de **Engenharia e Análise de Dados aplicada à Inteligência Artificial**.

O objetivo é estruturar um processo de análise de feedbacks de alunos, transformando comentários não estruturados em informações organizadas e úteis para apoiar decisões relacionadas à melhoria de cursos e da experiência de aprendizagem.

A primeira etapa do projeto concentra-se na **engenharia do prompt**, definindo a intenção da análise, o contexto dos dados, os critérios de análise e as restrições que devem orientar a IA.

<br>

## 🎯 Objetivo

Analisar avaliações e comentários de alunos sobre cursos online para identificar:

* Pontos positivos;
* Reclamações recorrentes;
* Dificuldades encontradas pelos alunos;
* Sentimentos predominantes;
* Temas recorrentes;
* Oportunidades de melhoria;
* Possíveis ações para a equipe responsável pelos cursos.

O resultado deverá transformar feedbacks individuais em **insights estruturados e acionáveis**.

<br>

## 👥 Público-alvo

Os resultados da análise são destinados principalmente a:

* Equipes responsáveis pelos cursos;
* Equipes de produtos educacionais;
* Coordenadores de conteúdo;
* Equipes de experiência do aluno.

A análise pode apoiar decisões relacionadas à atualização de conteúdos, melhoria da didática, materiais de apoio e experiência geral dos alunos.

<br>

## 🧩 Estrutura do desafio

O desenvolvimento do projeto foi dividido em etapas para construir progressivamente uma instrução mais precisa para a IA.

### 1. Definição da intenção

Nesta etapa foram definidos:

* O tipo de feedback analisado;
* O objetivo da análise;
* O público que utilizará os resultados;
* A decisão que a análise deverá apoiar;
* O formato esperado da entrega.

📄 Documento: [`docs/01-intention.md`](docs/01-intention.md)

<br>

### 2. Contexto e restrições

Nesta etapa foram adicionadas informações necessárias para orientar a IA, incluindo:

* Contexto dos cursos online;
* Estrutura esperada da base;
* Critérios de classificação;
* Cuidados com dados pessoais;
* Prevenção de conclusões sem evidências;
* Tratamento de dados insuficientes.

📄 Documento: [`docs/02-context-and-constraints.md`](docs/02-context-and-constraints.md)

<br>

### 3. Prompt final

As definições anteriores foram consolidadas em um único prompt estruturado, contendo:

* Papel da IA;
* Objetivo;
* Contexto;
* Dados disponíveis;
* Instruções de análise;
* Formato da resposta;
* Restrições.

📄 Documento: [`docs/03-final-prompt.md`](docs/03-final-prompt.md)

<br>

## 📊 Dados utilizados

A base planejada para o projeto contém informações anonimizadas sobre avaliações de alunos.

| Campo              | Descrição                             |
| ------------------ | ------------------------------------- |
| `aluno_id`         | Identificador anônimo do aluno        |
| `data_avaliacao`   | Data em que o feedback foi registrado |
| `curso`            | Nome do curso avaliado                |
| `categoria`        | Categoria ou área do curso            |
| `nota`             | Nota atribuída pelo aluno, de 1 a 5   |
| `comentario`       | Texto escrito pelo aluno              |
| `status_conclusao` | Indica se o aluno concluiu o curso    |

> Os dados pessoais dos alunos não fazem parte da análise.

<br>

## 🔎 Critérios de análise

Os feedbacks deverão ser analisados considerando:

### Tema

Identificação dos principais assuntos mencionados nos comentários.

Exemplos:

* Conteúdo;
* Didática;
* Professor;
* Material de apoio;
* Exercícios;
* Plataforma;
* Dificuldade;
* Carga horária.

### Sentimento

Classificação do sentimento predominante:

* Positivo;
* Negativo;
* Neutro;
* Misto, quando aplicável.

### Satisfação

A nota atribuída pelo aluno deverá ser considerada juntamente com o conteúdo textual do feedback.

### Recorrência

Os comentários deverão ser agrupados por temas para identificar padrões e diferenciar problemas isolados de ocorrências recorrentes.

<br>

## 📋 Resultado esperado

A análise deverá produzir uma saída estruturada contendo:

1. Resumo executivo;
2. Principais temas identificados;
3. Sentimentos predominantes;
4. Pontos positivos;
5. Principais problemas;
6. Evidências encontradas nos comentários;
7. Oportunidades de melhoria;
8. Recomendações práticas.

Exemplo de estrutura:

| Tema       | Sentimento | Ocorrências | Evidência                             | Oportunidade                  |
| ---------- | ---------- | ----------: | ------------------------------------- | ----------------------------- |
| Didática   | Negativo   |          18 | Alunos relatam ritmo acelerado        | Revisar ritmo das aulas       |
| Conteúdo   | Positivo   |          32 | Conteúdo considerado completo         | Manter estrutura atual        |
| Exercícios | Negativo   |          11 | Exercícios considerados insuficientes | Adicionar atividades práticas |

> Os valores acima são apenas ilustrativos e não representam resultados reais.

<br>

## 🛡️ Restrições e cuidados

A análise deverá seguir algumas regras:

* Utilizar somente os dados fornecidos;
* Não inventar números, comentários ou conclusões;
* Não expor dados pessoais ou sensíveis;
* Não generalizar uma opinião isolada;
* Não ignorar feedbacks negativos ou positivos;
* Diferenciar fatos de interpretações;
* Informar quando os dados forem insuficientes;
* Basear recomendações nas evidências encontradas.

<br>

## 🗂️ Estrutura do projeto

```text
project-ai-course-feedback-analysis/
│
├── README.md
│
├── docs/
    ├── 01-intention.md
    ├── 02-context-and-constraints.md
    └── 03-final-prompt.md
```

<br>

## 🚀 Próximas etapas

* [ ] Definir ou criar uma base de feedbacks para teste;
* [ ] Executar o prompt com os dados;
* [ ] Avaliar a qualidade das respostas da IA;
* [ ] Identificar possíveis erros ou inconsistências;
* [ ] Refinar o prompt;
* [ ] Comparar resultados antes e depois do refinamento;
* [ ] Estruturar os resultados em formato tabular;
* [ ] Criar visualizações dos principais indicadores;
* [ ] Documentar os insights obtidos.

<br>

## 🧠 Conceitos praticados

* Prompt Engineering;
* Análise de dados;
* Análise de sentimentos;
* Classificação de texto;
* Identificação de padrões;
* Geração de insights;
* Data Quality;
* Privacidade de dados;
* Tomada de decisão baseada em dados;
* Inteligência Artificial aplicada à análise de dados.

<br>


## 👨‍💻 Expert

<p>
    <img 
      align=left 
      margin=10 
      width=80 
      src="https://avatars.githubusercontent.com/u/44624583?v=4"
    />
    <p>&nbsp&nbsp&nbspMarcos Winther<br>
    &nbsp&nbsp&nbsp
    <a href="https://github.com/MarcosWinther">
    GitHub</a>&nbsp;|&nbsp;
    <a href="https://www.linkedin.com/in/marcoswinthersilva/">LinkedIn</a>
    </p>
</p>
<br/><br/>
