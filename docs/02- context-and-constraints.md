# 🧱 Passo 2 — Contexto e restrições

<br>

## Contexto

Estou trabalhando com feedbacks de alunos relacionados a cursos online, considerando aspectos como qualidade do conteúdo, didática dos professores, dificuldade das aulas, materiais de apoio e experiência geral com o curso.

<br>

## Dados disponíveis

A base contém:

| Campo              | Descrição                      |
| ------------------ | ------------------------------ |
| `aluno_id`         | Identificação anônima do aluno |
| `data_avaliacao`   | Data da avaliação              |
| `curso`            | Nome do curso                  |
| `categoria`        | Categoria do curso             |
| `nota`             | Nota de 1 a 5                  |
| `comentario`       | Comentário escrito pelo aluno  |
| `status_conclusao` | Status de conclusão do curso   |

<br>

## Critérios de análise

A IA deverá classificar os feedbacks considerando:

* Tema;
* Sentimento;
* Nível de satisfação;
* Problemas identificados;
* Pontos positivos;
* Recorrência dos temas.

<br>

## Cuidados e restrições

* Usar apenas os dados fornecidos;
* Não inventar números, causas ou conclusões;
* Não atribuir sentimentos sem evidência;
* Não expor dados pessoais;
* Não considerar uma opinião isolada como padrão;
* Não ignorar avaliações negativas ou positivas;
* Diferenciar fatos de interpretações;
* Informar limitações quando os dados forem insuficientes;
* Utilizar linguagem simples, objetiva e orientada à tomada de decisão.
