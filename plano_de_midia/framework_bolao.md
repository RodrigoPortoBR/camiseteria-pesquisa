# Framework: Análise por Chamada — Bolão CazéTV | Copa 2026

> **Produto:** Bolão de palpites da CazéTV, hospedado dentro do iFood, com mecânica de palpites por jogo (resultado 1x2, placar exato, palpites especiais), rankings, ligas privadas e gamificação. Plataforma white-label fornecida pela **LiveLike**. Meta de escala: 10M+ participantes na Copa.

> **Canais de chamada:** Os mesmos 20 canais do `mapa_de_midia.md` — todos os perfis CazéTV. A agência analisa e mede; não cria conteúdo.

---

## Diferença em relação à Camiseteria

| Dimensão | Camiseteria | Bolão |
|---|---|---|
| **Produto** | Transacional — compra única por pessoa | Recorrente — palpite a cada jogo (104 jogos) |
| **Destino do link** | Loja CazéTV no Mercado Livre | Bolão CazéTV no iFood (deep link) |
| **Conversão primária** | Pedido realizado | Cadastro no bolão + primeiro palpite feito |
| **Conversão recorrente** | N/A | Palpite feito a cada jogo (retenção) |
| **Urgência temporal** | Contínua | **Alta — palpite fecha no apito inicial de cada jogo** |
| **Virality loop** | Baixo (produto físico) | Alto — ligas privadas, convite de amigos, ranking compartilhável |
| **Analytics de destino** | GA4 + ML Analytics | iFood Analytics / Deep Link Tracker |

---

## O Funil do Bolão

```
┌─────────────────────────────────────────────────────────┐
│                        CHAMADA                          │
│          (post, story, live, tweet, mensagem...)        │
└─────────────────────┬───────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────┐
│  ESTÁGIO 1 — EXPOSIÇÃO                                  │
│  Impressões / Alcance / Visualizações                   │
│  → Quantas pessoas foram expostas à chamada?            │
└─────────────────────┬───────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────┐
│  ESTÁGIO 2 — INTERESSE (CTR)                            │
│  Cliques no link / QR scans / Taps no sticker           │
│  → Quantas pessoas clicaram para ir ao bolão no iFood?  │
└─────────────────────┬───────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────┐
│  ESTÁGIO 3 — ACESSO AO BOLÃO NO IFOOD                   │
│  Sessões na página do bolão rastreadas via UTM /        │
│  deep link com parâmetros                               │
│  → Quantos chegaram ao bolão dentro do iFood?           │
└─────────────────────┬───────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────┐
│  ESTÁGIO 4 — CADASTRO / ATIVAÇÃO                        │
│  Registros completados no bolão                         │
│  → Quantos se cadastraram? (usuários novos vs.          │
│    usuários iFood já existentes que aderiram)           │
└─────────────────────┬───────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────┐
│  ESTÁGIO 5 — PRIMEIRO PALPITE (Conversão Primária)      │
│  Palpite enviado no jogo em questão                     │
│  → % dos cadastrados que efetivamente palpitaram?       │
│    Esse é o indicador de ativação real.                 │
└─────────────────────┬───────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────┐
│  ESTÁGIO 6 — RETENÇÃO (Conversão Recorrente)            │
│  Usuário volta e palpita nos jogos seguintes            │
│  → Taxa de retorno jogo a jogo. Liga privada criada?    │
│    Amigos convidados? Posição no ranking compartilhada? │
└─────────────────────────────────────────────────────────┘
```

---

## Indicadores Universais do Bolão por Chamada

| Estágio | Indicador | Definição | Como rastrear |
|---|---|---|---|
| Exposição | Impressões / Alcance | Pessoas expostas à chamada | Analytics nativo do canal |
| Interesse | CTR da chamada (%) | Cliques / Impressões | Analytics nativo |
| Interesse | Cliques absolutos | Número de cliques no link / QR | Analytics nativo + rastreador |
| Acesso | Sessões no bolão iFood | Visitas à página do bolão rastreadas | iFood Analytics + UTM / deep link |
| Acesso | Taxa de drop CTR → Sessão | Cliques vs. sessões — identifica link quebrado ou fricção no iFood | UTM / deep link |
| Ativação | Cadastros no bolão | Novos registros com origem rastreada | iFood Analytics / plataforma do bolão |
| Ativação | Taxa de cadastro (%) | Cadastros / Sessões | iFood + plataforma bolão |
| Conversão | Palpites feitos por chamada | Palpites enviados com origem rastreada à chamada | Plataforma bolão + UTM |
| Conversão | Taxa de ativação (%) | Palpites / Cadastros | Plataforma bolão |
| Retenção | Taxa de retorno jogo seguinte | % dos ativados que palpitaram no próximo jogo | Plataforma bolão |
| Virality | Ligas privadas criadas | Usuários que criaram liga e convidaram amigos | Plataforma bolão |
| Virality | Convites aceitos (k-factor) | Amigos que entraram via convite por liga | Plataforma bolão |

---

## Timing de Análise — O Pré-Jogo é Crítico

Diferente da camiseteria (compra pode acontecer a qualquer momento), o bolão tem um **deadline hard: o apito inicial de cada jogo**. Depois que o jogo começa, palpitar naquele jogo não é mais possível. Isso muda a urgência da análise:

| Janela | Ação de análise | O que monitorar |
|---|---|---|
| **D-1 (véspera do jogo)** | Verificar se chamadas pré-jogo foram publicadas | CTR inicial, acesso ao iFood, cadastros |
| **H-3h (3h antes do jogo)** | Janela de pico — chamadas de conversão são publicadas aqui | CTR real-time, sessões iFood, palpites em andamento |
| **H-1h (última hora)** | Janela de urgência — "faltam 60 minutos para fechar!" | Pico de CTR e ativação |
| **Apito inicial** | Deadline — palpites fecham | Consolidar: total de palpites, cadastros, sessões atribuídos à chamada |
| **D+1 pós-jogo** | Relatório pós-jogo do bolão | Funil completo, taxa de ativação, comparativo com jogo anterior |
| **Semanal** | Análise de retenção | % de usuários que palpitou em todos os jogos da semana |

### Canais com análise urgente antes do kickoff

| Canal | Timing | Ação possível |
|---|---|---|
| YouTube Live (transmissão) | ✅ Real-time | QR code do bolão na arte; mensagem fixada no chat com link; CTA verbal |
| TikTok Live | ✅ Real-time | CTA verbal e link na descrição da live |
| Instagram Stories | ⚡ H-2h / H-1h | Story com countdown sticker + link do bolão |
| Twitter / X | ⚡ H-3h / H-1h | Tweet "faltam X horas para fechar o palpite" — monitorar engajamento |
| WhatsApp Comunidade | ⚡ H-2h | Mensagem de lembrete com link — open rate visível em horas |
| TikTok Vídeos | ⚡ H-3h | Vídeo publicado antes do jogo com CTA urgente |

---

## Rastreabilidade: UTMs + Deep Links iFood

Padrão recomendado para o bolão:

```
https://ifood.com.br/bolao-cazétv?
  utm_source=[canal]
  &utm_medium=[formato]
  &utm_campaign=bolao-copa2026
  &utm_content=[identificador-da-chamada]
```

**Exemplos:**

| Chamada | UTM |
|---|---|
| YouTube Live — Pré-jogo Brasil × Argentina | `utm_source=youtube&utm_medium=live&utm_campaign=bolao-copa2026&utm_content=pre-jogo-brasil-arg-jogo52` |
| Instagram Story — H-2h antes do jogo | `utm_source=instagram&utm_medium=story&utm_campaign=bolao-copa2026&utm_content=story-h2-jogo52` |
| WhatsApp Comunidade — Lembrete pré-jogo | `utm_source=whatsapp&utm_medium=comunidade&utm_campaign=bolao-copa2026&utm_content=msg-lembrete-jogo52` |
| Twitter — Tweet urgência H-1h | `utm_source=twitter&utm_medium=tweet&utm_campaign=bolao-copa2026&utm_content=tweet-h1-jogo52` |

> **Nota:** Verificar com iFood se deep links com parâmetros UTM são suportados na integração da plataforma do bolão. Se não, usar short links rastreáveis (Bitly/Rebrandly) que redirecionam para o bolão com UTMs.

---

## Loop de Otimização por Chamada — Bolão

```
┌──────────────────────────────────────────┐
│     CHAMADA PRÉ-JOGO PUBLICADA           │
└──────────────┬───────────────────────────┘
               │
               ▼
   ┌──────────────────────────┐
   │   LEITURA DO FUNIL       │
   │  Exposição → CTR →       │
   │  Sessões iFood →         │
   │  Cadastros → Palpites    │
   └───────────┬──────────────┘
               │
       ┌───────┴────────┐
       │                │
       ▼                ▼
 CTR acima         CTR abaixo
 do benchmark      do benchmark
       │                │
       ▼                ▼
  Documentar        Diagnosticar:
  como padrão       • A chamada tem urgência clara? ("fecha hoje!")
  + replicar        • O link do bolão está visível e funcionando?
                    • A arte comunica que é para o jogo DE HOJE?
                    • Horário de publicação foi adequado?
                    • Faltou mostrar o prêmio / ranking?
                         │
                         ▼
                    Ajustar nas próximas
                    chamadas pré-jogo

⚠️  Para o bolão, o tempo de aprendizado é limitado:
    há um jogo novo a cada ~1-2 dias durante a Copa.
    Otimizações devem ser aplicadas no jogo seguinte.
```

### O que investigar quando o funil do bolão quebra

| Estágio com queda | Hipótese a investigar |
|---|---|
| Impressões baixas | Publicação fora da janela pré-jogo; algoritmo não distribuiu a tempo |
| CTR baixo com impressões altas | Chamada sem urgência ("faz o palpite" vs. "fecha em 2h!"); arte não comunica o jogo |
| Sessões iFood baixas apesar de CTR alto | Link errado, deep link não funciona no iOS/Android, iFood com lentidão |
| Cadastros baixos apesar de sessões | Friction no onboarding do bolão dentro do iFood; UX da plataforma LiveLike — verificar fluxo de cadastro no ambiente iFood |
| Palpites baixos apesar de cadastros | Usuário cadastrou mas não entendeu o fluxo de palpite; experiência confusa |
| Retenção baixa no jogo seguinte | Usuário não foi notificado; sem liga privada criada; sem engagement pós-resultado |

---

## Indicadores de Retenção e Virality — Análise Semanal

Esses indicadores não são rastreáveis por chamada individual — são analisados em nível de produto/plataforma com periodicidade semanal e por rodada de jogos:

| Indicador | Definição | Periodicidade |
|---|---|---|
| DAU / WAU do bolão | Usuários ativos por dia / semana | Semanal |
| Taxa de palpite por usuário ativo | Média de palpites por jogo por usuário | Semanal |
| Taxa de retenção D+7 | % dos cadastrados na semana 1 que palpitaram na semana 2 | Semanal |
| Ligas privadas criadas | Número de ligas criadas e ativas | Semanal |
| K-factor (convites aceitos / convites enviados) | Indicador de virality orgânica | Semanal |
| Net growth de participantes | Novos cadastros - cancelamentos | Semanal |
| Share de ranking | Vezes que o ranking foi compartilhado | Semanal |

---

*7 de maio de 2026 — Versão 1.0*
