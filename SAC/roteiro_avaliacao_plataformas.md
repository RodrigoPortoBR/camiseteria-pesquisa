# 🔍 Roteiro de Avaliação de Plataformas — SAC Bot CazéTV

> **Contexto para o fornecedor:** Operação de SAC para venda de uniformes durante a Copa do Mundo FIFA 2026. Duração: ~3 meses (Mai–Jul 2026). Canal principal: Instagram DM. Volume estimado: 3.000–6.000 DMs. Bot deve responder em PT-BR com base em Knowledge Base. Handoff automático para agente humano quando necessário.

---

## Critérios de Decisão (pesos)

| Critério | Peso |
|---|---|
| Qualidade do bot em PT-BR (linguagem natural) | 🔴 Alta |
| Tempo de implementação | 🔴 Alta |
| Custo total para 3 meses | 🔴 Alta |
| Handoff automático bot → humano | 🟡 Média |
| Integração com Instagram (DM nativo) | 🔴 Alta |
| Facilidade de configurar a Knowledge Base | 🟡 Média |
| Suporte em português | 🟢 Baixa |

---

## Perguntas para ambas as plataformas

### 1. Contrato e Custo
- Vocês oferecem contratos mensais (sem anualidade obrigatória)?
- Qual o custo total para 3 meses de uso para uma operação de SAC com até 6.000 DMs?
- Existem custos extras por volume de mensagens, por agente humano adicional ou por integração com Instagram?
- Qual é o período mínimo de contrato?

### 2. Implementação
- Qual o prazo mínimo estimado para ir ao ar, do zero à operação, para um caso como o nosso?
- Vocês oferecem suporte de implementação incluso ou é cobrado à parte?
- Existe um processo de onboarding guiado ou é self-service?

### 3. Instagram DM
- A integração com Instagram DM é nativa ou depende de terceiros (ex: Zapier)?
- Há alguma limitação da API do Instagram que afete o volume ou o tempo de resposta?
- O bot consegue responder DMs sem intervenção humana, de forma totalmente autônoma?

### 4. Handoff Humano
- Como funciona o handoff do bot para o agente humano? É automático ou precisa de configuração especial?
- O agente humano recebe o histórico completo da conversa antes de assumir?
- É possível definir critérios customizados para o acionamento do handoff (ex: quando o bot não tiver resposta na KB)?

### 5. Knowledge Base e IA
- O bot usa LLM (linguagem natural) para responder com base na KB, ou funciona por menus/fluxos/keywords?
- Como é o processo de alimentar a Knowledge Base? É via upload de documento, formulário ou API?
- Se a KB não tiver a resposta, o bot escala automaticamente ou responde algo genérico?

---

## Perguntas específicas por plataforma

### 🟣 ManyChat

| # | Pergunta | Por que perguntar |
|---|---|---|
| 1 | Vocês têm funcionalidade de IA generativa (LLM) integrada ao bot de Instagram ou é apenas fluxo de botões/keywords? | ManyChat é historicamente baseado em fluxos — verificar se evoluíram para LLM real |
| 2 | Se for por fluxo: quantos fluxos distintos um bot típico desta operação teria, e quanto tempo leva para configurar? | Dimensionar esforço de implementação |
| 3 | Se o cliente mandar uma mensagem fora dos fluxos configurados, o que acontece? | Verificar comportamento no "caso não mapeado" |
| 4 | Vocês têm cases de uso parecidos (e-commerce de produto físico, volume alto de DMs, operação temporária)? | Validar fit da plataforma |
| 5 | Qual a diferença real entre o plano Pro e os planos superiores para o nosso caso? | Entender se plano básico já resolve |

### 🔵 Respond.io

| # | Pergunta | Por que perguntar |
|---|---|---|
| 1 | O AI Agent do Respond.io funciona com instrução em português? Vocês têm cases de uso em PT-BR? | Qualidade do LLM em português é crítica |
| 2 | Como funciona a KB na prática — eu subo um PDF/documento ou preciso estruturar por perguntas e respostas? | Impacto direto na velocidade de implementação |
| 3 | Qual o modelo de LLM embarcado (GPT-4, Claude, próprio)? Posso trocar? | Qualidade das respostas |
| 4 | Existe um sandbox ou trial para testar a qualidade do bot antes de contratar? | Reduz risco de contratar e decepção depois |
| 5 | O plano mensal permite cancelamento sem multa? | Garantir saída limpa em 31 Jul sem custo extra |

---

## Teste Prático Obrigatório (antes de decidir)

> [!IMPORTANT]
> **Não contrate sem fazer o teste abaixo.** A qualidade do bot em PT-BR varia muito entre plataformas e não é perceptível só pelo site.

Envie estas 5 perguntas para o bot de demonstração que cada fornecedor oferecer:

1. `"Qual o maior tamanho disponível e quais as medidas?"`
2. `"Comprei um uniforme GG mas quero trocar por XGG, como faço?"`
3. `"Meu pedido está atrasado e a Copa começa em 3 dias, o que vocês podem fazer?"`
4. `"Posso colocar meu nome nas costas do uniforme?"`
5. `"Quero falar com um atendente humano"`

**O que avaliar em cada resposta:**
- A linguagem soou natural em português ou mecânica/robótica?
- Respondeu com precisão ou deu resposta genérica?
- Na pergunta 3 (urgência emocional), o bot demonstrou empatia?
- Na pergunta 5, o handoff aconteceu rapidamente e com contexto?

---

## Matriz de Decisão Final

Preencher após reunião/teste com cada fornecedor:

| Critério | ManyChat | Respond.io | Peso | Vencedor |
|---|---|---|---|---|
| Qualidade do bot PT-BR | /10 | /10 | 30% | |
| Tempo de implementação | /10 | /10 | 25% | |
| Custo total 3 meses | /10 | /10 | 25% | |
| Handoff automático | /10 | /10 | 10% | |
| Facilidade de configuração | /10 | /10 | 10% | |
| **TOTAL PONDERADO** | | | 100% | |

---

*30 de março de 2026 — Decisão deve ser tomada até 15 de Abril de 2026*
