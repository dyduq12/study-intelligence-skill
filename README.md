# Study Intelligence Miner - Agent Skill

![Autor](https://img.shields.io/badge/Autor-Eduardo%20Borborema%20Brito-blue)
![Licença](https://img.shields.io/badge/Licen%C3%A7a-Source--Available%20%26%20Non--Commercial-red)
![Compatibility](https://img.shields.io/badge/Compatibility-Antigravity%20%7C%20Claude%20%7C%20Gemini%20%7C%20Cursor-brightgreen)
![Output](https://img.shields.io/badge/Output-MindNote%20Engine%20Validated-darkgreen)

Uma **Agent Skill universal de engenharia de dados e análise cognitiva** projetada para permitir que agentes de inteligência artificial (Google Antigravity, Claude Code, Gemini CLI, Cursor, Copilot Workspace) processem acervos desordenados de materiais de estudo, apliquem filtros interativos de anti-ruído, classifiquem competências em profundidade e sintetizem **Mapas Mentais** e **Cronogramas Táticos** compatíveis com o **MindNote Engine**.

---

## 🎯 O que esta Skill Faz?

Diante de um diretório contendo dezenas ou centenas de arquivos (PDFs de provas, apostilas, slides, notas ou simulados), a skill assume o papel de um engenheiro de dados cognitivo:

1. **Conduz uma entrevista rápida de escopo (Fase 0)**:
   - *Alvo de estudo*: Qual é a prova, concurso, certificação ou disciplina?
   - *Filtros de exclusão (Anti-Ruído)*: O que descartar sumariamente? (ex: outras bancas, legislações revogadas, matérias secundárias).
   - *Arquivos brutos e horizonte temporal*: Onde estão os dados e qual o prazo de revisão?
2. **Deduplicação Estrutural**:
   - Agrupa arquivos repetidos com nomes diferentes através de hashing de blocos textuais iniciais.
3. **Classificação Semântica Profunda**:
   - Analisa o cerne da competência exigida em cada documento/questão, rejeitando buscas ingênuas por palavras-chave isoladas.
4. **Priorização de Pareto**:
   - Separa os tópicos em:
     - **Nível 1 - CRUCIAL (`#DC2626`)**: Os 10-20% de assuntos que respondem por 80% do retorno de pontuação.
     - **Nível 2 - ALTO IMPACTO (`#D97706`)**: Tópicos frequentes que consolidam diferenciais competitivos.
     - **Nível 3 - PERIFÉRICO (`#2563EB`)**: Tópicos de retorno marginal.
5. **Síntese no MindNote Engine com Validação Tripla**:
   - Gera o mapa mental completo e o cronograma tático diário com pautas de 3 linhas para fórmulas e macetes rápidos.

---

## 🚀 Como Instalar e Usar

### 1. No Google Antigravity / Gemini CLI
Copie a pasta desta skill para o seu diretório de configurações:
```bash
# Copiar para as skills do Antigravity / Gemini:
cp -r study-intelligence-skill ~/.gemini/config/skills/study-intelligence-miner
```

### 2. No Claude Code / Cursor / Agentes Customizados
Basta apontar para o arquivo [`SKILL.md`](SKILL.md) nas suas instruções de sistema ou carregar como instrução personalizada.

---

## 💬 Exemplo de Uso no Chat do Agente

Para ativar a skill, você pode simplesmente enviar:
```text
"Quero estudar para a Certificação AWS Solutions Architect usando esta pasta de apostilas e simulados. 
Ative a skill study-intelligence-miner para filtrar o que não cai, classificar os tópicos e gerar meu mapa mental no MindNote."
```

O agente imediatamente iniciará o protocolo com a entrevista de alinhamento e o pipeline em 5 fases.

---

## 📖 A História de Origem (The Origin Story)

Esta skill não nasceu em um laboratório teórico. Ela foi concebida por **Eduardo Borborema Brito** diante de um problema prático colossal: a necessidade de auditar e estruturar **mais de 5,56 GB de simulados em PDF** contendo **1.422 cadernos** para o 2º Dia do ENEM (Matemática e Ciências da Natureza).

Ao tentar analisar os cadernos brutos, o cenário era de puro ruído: centenas de simulados da Fuvest, Unicamp e vestibulares paulistas estavam misturados nas pastas, e arquivos duplicados com nomes como "Versão Medicina" e "Caderno Azul" inflariam as estatísticas se fossem contados duas vezes.

Para superar essa barreira, Eduardo estruturou uma força-tarefa multiagente que:
- Eliminou cirurgicamente **920 cadernos contaminantes**.
- Deduplicou os exames por hash das primeiras questões em **719 edições canônicas**.
- Extraiu e classificou o texto integral de **24.419 questões autênticas**.
- Revelou padrões estatísticos definitivos, como o fato de que **Matemática Básica e Proporcionalidade respondem por 48,92% de toda a prova de Matemática**.

O sucesso estrondoso desse case real provou que a metodologia funcionava em escala industrial. Eduardo decidiu então abstrair todo o método, transformando a esteira analítica nesta **Agent Skill universal e reutilizável**, para que qualquer estudante, concurseiro ou profissional de tecnologia possa aplicar o mesmo rigor de mineração de dados a qualquer exame ou matéria do mundo.

👉 **Conheça o estudo de caso completo e os gráficos estatísticos das 24.419 questões**:  
[https://github.com/dyduq12/enem-dia2-case-study](https://github.com/dyduq12/enem-dia2-case-study)

---

## ⚖️ Propriedade Intelectual e Licença

Esta skill e sua metodologia foram criadas e desenvolvidas por **Eduardo Borborema Brito**.

Este projeto é protegido pela licença **[Eduardo Borborema Source-Available & Non-Commercial License 1.0](LICENSE)**.  
Uso livre para fins educacionais, estudos pessoais e aprendizado não-comercial. É expressamente proibida a apropriação indevida de autoria ou qualquer forma de exploração comercial sem autorização prévia por escrito do autor.
