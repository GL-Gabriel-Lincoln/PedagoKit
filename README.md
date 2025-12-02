# PedagoKit — Gestor Inteligente de Grupos

O PedagoKit é uma ferramenta desenvolvida para resolver uma das tarefas logísticas mais chatas (e estratégicas) do professor: **criar grupos de trabalho eficientes**. 

Diferente de sorteadores comuns, este projeto permite criar grupos com critérios pedagógicos reais, como equilibrar notas, misturar gêneros ou respeitar regras de convivência (quem não pode trabalhar junto).

**Acesse a versão online:** [https://gl-gabriel-lincoln.github.io/PedagoKit/](https://gl-gabriel-lincoln.github.io/PedagoKit/)

---

## 🎯 O Que a Ferramenta Faz?

Nesta versão, o foco é total na **Ferramenta de Diagnóstico e Agrupamento**. Ela cobre 5 casos de uso essenciais para a sala de aula:

1.  **Aleatórios (Quebra-gelo):**
    * Mistura total da turma para atividades rápidas ou para integrar alunos que não se conhecem bem.
2.  **Baseados em Nota (Tutoria por Pares):**
    * Utiliza um algoritmo *Greedy* (Cobra) para garantir que todos os grupos tenham uma média de desempenho similar. Mistura alunos com facilidade e dificuldade para estimular a colaboração.
3.  **Baseados em Gênero:**
    * Distribui meninos e meninas equitativamente entre os grupos, evitando "o clube do bolinha" ou grupos segregados, ideal para dinâmicas sociais.
4.  **Aleatórios com Exceções (Gestão de Conflito):**
    * Você define quem **NÃO** pode ficar junto (coluna "Evitar"). O algoritmo monta os grupos respeitando essas restrições para evitar conversas paralelas ou brigas.
5.  **Intencionais com Pré-definições:**
    * Você define quem **DEVE** ficar junto (coluna "Juntar"). Ideal para quando você já tem duplas formadas e quer apenas completar os grupos, ou para garantir apoio a alunos com necessidades específicas.

Além disso, a ferramenta mantém a **Análise de Impacto**, mostrando onde a intervenção pedagógica é mais necessária com base nas notas da turma.

---

## 📋 Como Usar (Novo Formato de Dados)

Para que a mágica das "Regras" e "Gênero" aconteça, a lista de alunos aceita novas colunas opcionais.

**Formato do CSV / Texto:**
`Nome, Gênero, Evitar, Juntar, Nota1, Nota2...`

**Exemplo de preenchimento:**
```csv
Ana, F, , Bia, 9.0, 9.5      (Ana é menina, deve ficar com a Bia)
Bia, F, , Ana, 6.0, 5.5      (Bia é menina, deve ficar com a Ana)
Carlos, M, João, , 5.0, 4.0  (Carlos evita o João)
João, M, Carlos, , 8.0, 8.5  (João evita o Carlos)
Pedro, M, , , 7.0, 7.5       (Pedro sem restrições)