# 🔍 SM4 - Engenharia Reversa de Prompts

## 📝 Visão Geral do Projeto
Este projeto investigou os mecanismos internos de resposta das IAs através da **Engenharia Reversa**. O objetivo foi desconstruir como modelos de linguagem (LLMs) processam camadas de contexto, persona e restrições para prever resultados específicos em tarefas criativas e técnicas.

Desenvolvido para a disciplina de **Engenharia de Prompt e Aplicações em IA (2026.1)**.

---

## 🧪 Experimentos e Metodologia

### 🎨 1. Geração Iterativa de Imagens (Visão Computacional)
Análise de como a IA mantém a consistência visual através de refinamentos sucessivos de um prompt base:
* **Prompt Base:** Astronauta em Marte tocando violoncelo no estilo barroco.
* **Refinamento Progressivo:** Inclusão de elementos de cena (ETs na plateia), ajuste de enquadramento (arquibancadas) e controle de cenário (remoção de cortinas).
* **Conclusão:** A IA demonstra uma forte capacidade de manter o contexto "persistente", mas pequenas variações semânticas podem causar mudanças drásticas na composição final.

### ✍️ 2. Arquitetura de Persona e Tom (NLP)
Simulação de e-mails entre um Pirata e um Rei para testar a flexibilidade do modelo em adaptar o **contexto emocional**:
* **Fluxo:** Do e-mail formal padrão à introdução de elementos de ficção (7 esferas do dragão) e personas de extrema arrogância.
* **Teste de Restrição:** Manter o formato de "pedido de desculpas" enquanto a persona agia de forma provocativa.
* **Conclusão:** O "comportamento" da IA é uma resposta direta à densidade do contexto fornecido no prompt (Few-shot/Zero-shot prompting).

---

## 📊 Matriz de Aprendizados
| Elemento Analisado | Impacto no Output | Observação Técnica |
| :--- | :---: | :--- |
| **Persona** | Crítico | Altera o vocabulário e a estrutura sintática. |
| **Contexto** | Alto | Define os limites do universo criativo da IA. |
| **Restrições** | Médio | Testa a aderência do modelo às regras negativas (o que não fazer). |
| **Iteração** | Constante | Demonstra a memória de curto prazo do modelo durante a sessão. |

---

## 🚀 Tecnologias Utilizadas
* **Modelo:** Qwen 3.5 Plus (Alibaba Cloud).
* **Plataforma:** chat.qwen.ai.
* **Técnicas:** Chain-of-Thought (CoT) e Role-playing Prompting.

---

## 🏆 Veredito Técnico
A Engenharia Reversa provou que a IA não "compreende" conceitos, mas sim **prevê padrões** baseados nas restrições fornecidas. Dominar esses limites permite que o desenvolvedor crie aplicações mais robustas e previsíveis.
