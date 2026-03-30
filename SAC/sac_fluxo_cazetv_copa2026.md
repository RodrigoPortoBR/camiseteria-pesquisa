# 🎽 SAC CazéTV — Estrutura de Atendimento | Copa 2026

> **Estratégia:** Mínimo de pessoas, máximo de automação. Bot de IA resolve o Instagram. Humanos dedicados ao que o Mercado Livre não consegue resolver sozinho.

---

## 1. O Tamanho do Desafio

| Etapa | Referência | Estimativa |
|---|---|---|
| Pedidos totais | Meta da operação | 400.000 |
| Taxa de contato no Meli (benchmark BR) | ~12–18% dos pedidos | ~60.000 contatos |
| Transbordo para SAC CazéTV (15% do Meli) | 15% de 60.000 | **~9.000 tickets humanos** |
| Instagram DMs sobre camiseteria | Estimativa conservadora | **~3.000–6.000 msgs** |
| **Bot resolve (est. 70%)** | | ~2.000–4.200 resolvidos por IA |
| **Escalados para humano (30%)** | | **~900–1.800 casos humanos** |

> [!CAUTION]
> A Copa amplifica **tudo**. Um uniforme atrasado viralizado no X antes de Brasil x Argentina pode gerar cobertura de mídia. SAC bem estruturado é proteção de marca, não só resolução de ticket.

```
📅 Janela de pressão (~3 meses de operação)

1 MAI  → GO LIVE da Camiseteria + SAC ativo
11 JUN → Copa começa ← DEADLINE HARD de entrega
          Todos os 104 jogos ao vivo no YouTube (gratuito)
          CazéTV no centro das atenções
19 JUL → Final da Copa
31 JUL → Encerramento do SAC
```

---

## 2. Estratégia por Canal

| Canal | Quem Atende | Lógica |
|---|---|---|
| **Instagram DM** | 🤖 Bot de IA (primário) + 👤 humano (escalada) | Volume alto, perguntas repetitivas → ideal para IA |
| **Meli Transbordo (15%)** | 👤 Humano obrigatório | Casos complexos exigem ação no sistema |

---

## 3. Estrutura da Equipe — Mínimo Viável

> [!TIP]
> Com o bot absorvendo ~70% do Instagram, a equipe humana pode focar no que realmente importa: os casos complexos do Meli.

| Posição | Qtd | Canal | Responsabilidade |
|---|---|---|---|
| **Coordenador SAC** | 1 | Todos | Gestão, configuração do bot, escaladas, relatórios |
| **Especialista Meli / Trocas** | 3–4 | Meli + Email | Transbordo complexo: troca, defeito, estorno, NF |
| **Agente Instagram (handoff)** | 1 | Instagram DM | Apenas casos que o bot não conseguir resolver |
| **Total** | **5–6** | | |

**Escala:**
- **Mai–10 Jun:** Seg–Sex 9h–18h; bot Instagram 24/7 autônomo
- **Copa (11 Jun–19 Jul):** Seg–Dom, 9h–21h em dias de jogo; bot ininterrupto
- **20–31 Jul:** Redução gradual, foco na cauda de devoluções

---

## 4. Fluxo — Mercado Livre (Transbordo Humano)

### Critérios de transbordo (o Meli sinaliza)

1. Pedido de troca de tamanho (Meli não opera troca direta)
2. Produto com defeito de fabricação (análise manual)
3. Reclamação aberta sem resolução no Meli
4. Solicitação de nota fiscal avulsa
5. Pedido cancelado com pagamento não estornado após 5 dias
6. Casos que atingiram mediação Meli (risco de reputação)

```
FLUXO TRANSBORDO MELI → SAC CazéTV

[1] Atendente Meli identifica caso de transbordo
         │
         ▼
[2] Abre ticket na plataforma SAC com:
    • ID do pedido Meli
    • Nome do cliente
    • Categoria do problema
    • Histórico da conversa Meli
         │
         ▼
[3] Especialista CazéTV recebe e age
         │
         ├─► Resolução → SLA 24h → responde ao cliente (Meli ou email)
         └─► Caso complexo → escala Coordenador → SLA 48h com aviso pro-ativo
```

### Categorias de ticket Meli

| Categoria | Exemplo | % Esperada |
|---|---|---|
| Logística / Entrega | Atraso, extravio | 40% |
| Troca de Tamanho | Cliente pediu tamanho errado | 25% |
| Defeito de Produto | Costura, estampa, tecido | 15% |
| Financeiro | Estorno, NF, cobrança dupla | 10% |
| Personalização | Pedido customizado com erro | 5% |
| Outros | | 5% |

---

## 5. Fluxo — Instagram DM (Bot de IA + Escalada Humana)

### Princípio
O bot responde **tudo sobre camiseteria** de forma autônoma via DM. Se não souber → escala para humano com contexto completo. Mensagens fora do tema camiseteria → bot ignora ou redireciona.

```
FLUXO INSTAGRAM DM

[1] Cliente envia DM
         │
         ▼
[2] BOT DE IA analisa intenção da mensagem
    Consulta a Knowledge Base da camiseteria:
    • Tabela de tamanhos e medidas
    • Política de troca e devolução
    • Status de entrega (integração rastreio)
    • FAQ produto, personalização, envio
         │
         ├─► Assunto = camiseteria com resposta disponível
         │     → Bot responde em < 2min, 24/7 ✅
         │
         ├─► Assunto ≠ camiseteria
         │     → Bot ignora ou redireciona ⏭️
         │
         └─► Sem contexto suficiente (pedido específico com problema)
               → Escalada automática 🚨
               → Agente humano recebe: histórico + intenção detectada
               → SLA: 4h (útil) / 2h (dia de jogo)
```

---

## 6. Base de Conhecimento do Bot

> [!IMPORTANT]
> A qualidade do bot depende diretamente da base de conhecimento. Estes documentos precisam estar prontos **antes** de ativar o bot.

| Documento | Conteúdo | Responsável |
|---|---|---|
| Tabela de tamanhos | Grade M/F/infantil com medidas em cm | Operações |
| Política de troca/devolução | Prazo, condições, como iniciar | Jurídico / Ops |
| Guia de rastreio | Como rastrear, link, prazo por região | Logística |
| FAQ pré-venda (20–30 perguntas) | Perguntas + respostas aprovadas | SAC + Produto |
| Política de personalização | O que personaliza, prazo extra, preço | Produto |
| Prompt de tom de voz | Como o bot deve falar (tom CazéTV) | Marketing |

---

## 7. SLAs

| Canal | Tipo | Meta |
|---|---|---|
| Instagram DM (bot) | Primeira resposta | < 2 min (24/7) |
| Instagram DM (humano, após escalada) | Primeira resposta | ≤ 4h (útil) / ≤ 2h (jogo) |
| Meli Transbordo | Primeira resposta | ≤ 24h |
| Meli Transbordo | Resolução final | ≤ 72h |

---

## 8. Tom de Voz e Scripts

**Princípios:**
- Próximo e humano — jamais robótico
- Transparente — se não tem resposta agora, diz quando terá
- Apaixonado pelo futebol — usa o contexto da Copa para empatia

**Bot — resposta a dúvida de tamanho:**
> "Oi! 🙌 Nossa tabela de tamanhos está aqui: [link]. Se quiser, me conta o seu peso e altura e eu te indico o tamanho certo pra você arrasar na Copa!"

**Humano — reclamação de atraso (DM):**
> "Oi [Nome]! 😕 Que situação chata, sinto muito. Me passa o número do pedido que eu verifico agora o que está acontecendo. A gente quer te ver com o uniforme antes da Copa começar!"

---

## 9. Plataformas Recomendadas — Filtro: 3 Meses, Rápido, Barato

> [!IMPORTANT]
> A operação dura **~3 meses** (Go Live Maio → 31 Jul 2026). O custo total da plataforma é o que importa, não o mensal. Critérios eliminatórios: **tempo de implementação > 4 semanas** ou **custo total 3 meses > R$ 10.000**.

### Comparativo com filtro operação curta

| Plataforma | Bot IA PT-BR | Instagram | Handoff Humano | Meli | Impl. rápida? | Custo total 3 meses (est.) | Recomendação |
|---|---|---|---|---|---|---|---|
| **ManyChat** | ⚠️ Fluxos (não LLM) | ✅ | ✅ | Via Zapier | ✅ < 1 semana | R$ 1.500–3.600 | ⭐ Melhor custo-benefício |
| **Respond.io** | ✅ LLM + KB | ✅ | ✅ | Via API | ✅ 1–2 semanas | R$ 2.400–6.000 | ⭐ Melhor IA conversacional |
| **Trengo** | ✅ | ✅ | ✅ | ✅ nativo | ✅ 1–2 semanas | R$ 3.000–9.000 | ✅ Boa opção com Meli nativo |
| **Gorgias** | ✅ | ✅ | ✅ | ✅ nativo | ⚠️ 2–4 semanas | R$ 4.500–12.000 | ❌ Caro para 3 meses |
| **Intercom** | ✅ Fin AI | ✅ | ✅ | Via API | ⚠️ 3–4 semanas | R$ 6.000–15.000 | ❌ Caro e demorado |

### Recomendação para esse projeto

**Cenário A — Prioridade: menor custo**
> **ManyChat** (bot por fluxo/regras) + canal humano via DM direta ou ferramenta gratuita de inbox  
> ⚠️ IA mais limitada — o bot responde por menus e keywords, não por linguagem natural livre

**Cenário B — Prioridade: melhor IA (recomendado)**
> **Respond.io** — LLM com base de conhecimento, Instagram nativo, handoff automático, implementação em 1–2 semanas, custo controlado para 3 meses

**Integração com Meli no Cenário B:**
> O Meli não precisa estar integrado à plataforma — o fluxo de transbordo pode ser gerenciado por email ou via inbox manual, já que são ~9.000 casos distribuídos em 3 meses (~100/dia). Isso simplifica a implementação sem prejudicar o SLA.

---

## 10. KPIs

| KPI | Meta | Frequência |
|---|---|---|
| Taxa de resolução autônoma do bot | ≥ 65% | Semanal |
| CSAT pós-atendimento | ≥ 85% | Semanal |
| TMR — Tempo Médio de Resolução (humano) | ≤ 48h | Semanal |
| Taxa de recontato (mesmo problema) | ≤ 10% | Quinzenal |
| Reputação Meli | ≥ Verde | Semanal |
| Tickets acima do SLA | 0 | Diário |

---

## 11. Cronograma de Implantação

> [!IMPORTANT]
> Janela total: **~3 meses** | Go Live Camiseteria: **Maio 2026** | Encerramento SAC: **31 Jul 2026**

| Fase | Período | Entregável | Prazo crítico |
|---|---|---|---|
| **Fundação** | 1–15 Abr | Escolher plataforma, contratar equipe mínima | ← Não pode atrasar |
| **Knowledge Base** | 15 Abr–5 Mai | Preencher base de conhecimento do bot por completo | ← Gargalo principal |
| **Configuração** | 5–20 Mai | Configurar bot, testar fluxos, aprovar scripts | |
| **Go Live** | 20 Mai 2026 | SAC ativo — bot no ar + equipe Meli operacional | ← Go Live Camiseteria |
| **Pré-Copa** | 20 Mai–10 Jun | Operação rodando, ajustes finos no bot | |
| **Copa** | 11 Jun–19 Jul | Escala reforçada, bot ininterrupto, relatórios diários | ← Pico máximo |
| **Encerramento** | 20–31 Jul | Trocas/devoluções cauda, encerramento de contratos | ← Fim da operação |

---

## 12. Riscos

| Risco | Probabilidade | Impacto | Plano |
|---|---|---|---|
| **Knowledge Base incompleta no Go Live** | Alta | Crítico | Iniciar preenchimento em Abr — não pode bloquear a config do bot |
| **Atraso na escolha da plataforma** | Média | Alto | Decidir até 15 Abr — cada semana perdida comprime o tempo de teste |
| Bot com resposta ruim em PT-BR | Média | Alto | Testar com perguntas reais antes de Mai; trocar se necessário |
| Volume de DMs acima do estimado | Média | Alto | Ajustar threshold de escalada do bot |
| Volume Meli > 100 tickets/dia | Baixa | Alto | Reforço pontual via BPO ou freelancer |
| Encerrar contratos no prazo (31 Jul) | Baixa | Médio | Negociar plataforma por 3 meses — evitar contratos anuais |

---

*30 de março de 2026 — Revisão recomendada: Maio 2026*
