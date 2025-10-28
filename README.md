# PedagoKit  pedagogical toolkit

Um pacote de ferramentas pedagógicas para auxiliar professores no planejamento, execução e avaliação da aula, desenvolvido como um projeto MVP (Produto Mínimo Viável).

**Acesse a versão online:** [https://gl-gabriel-lincoln.github.io/PedagoKit/](https://gl-gabriel-lincoln.github.io/PedagoKit/)

---

## ✨ Ferramentas Incluídas

Este MVP contém 3 ferramentas principais focadas em resolver "dores" pedagógicas:

1.  **Diagnosticar Turma (Gerador de Grupos & Análise de Impacto):**
    * Permite importar ou colar listas de alunos com notas (formato `Nome,nota1,nota2,...`).
    * Gera grupos balanceados otimizando para que as médias dos grupos fiquem próximas à média da turma (usando um algoritmo *greedy*).
    * **Análise de Impacto:** Identifica os alunos prioritários (menores médias) e aponta qual avaliação teve o pior desempenho *para esse grupo*, sugerindo o foco de intervenção com maior potencial matemático para elevar a média geral.

2.  **Planejar Aula (Estruturador 5E):**
    * Recebe a duração total da aula, o tópico e o objetivo.
    * O professor escolhe o foco da aula (Matéria Nova, Revisão/Prática, Avaliação).
    * Sugere uma divisão do tempo da aula nas 5 etapas do modelo 5E (Engajar, Explorar, Explicar, Elaborar, Avaliar), adaptando os tempos e descrições ao foco escolhido e aos dados inseridos.

3.  **Nivelar Perguntas (Taxonomia de Bloom):**
    * Recebe o tópico da aula e um contexto de aplicação (opcional).
    * O professor escolhe o objetivo cognitivo (Checagem Rápida, Gerar Discussão, Criar Desafio).
    * Gera perguntas baseadas na Taxonomia de Bloom, adaptadas ao tópico e contexto, nos níveis cognitivos correspondentes ao objetivo (Lembrar/Entender, Aplicar/Analisar, Avaliar/Criar).

## 🚀 Como Usar

1.  Acesse o [site online](https://gl-gabriel-lincoln.github.io/PedagoKit/).
2.  Use os links na barra de navegação para ir até a ferramenta desejada.
3.  Preencha os campos e clique nos botões para gerar os resultados.
4.  Na Ferramenta 1, você pode usar o botão "Exemplo" para preencher a lista de alunos rapidamente.

## 🛠️ Tecnologias Utilizadas

* HTML5 (Semântico e acessível)
* CSS3 (Design moderno e responsivo, com variáveis CSS)
* JavaScript (Vanilla JS, sem frameworks, para interatividade e lógica das ferramentas)
* GitHub Pages (Hospedagem)

## 🔮 Próximos Passos (Sugestões do MVP)

* Desenvolvimento de um backend (ex: Node.js) para salvar turmas e históricos.
* Autenticação de professores.
* Integração com APIs (ex: Google Classroom) para importar turmas.
* Dashboards visuais com gráficos (ex: Chart.js) para a análise da turma.

---

*Projeto desenvolvido por Gabriel Lincoln.*