# Mapa de Mídia — CazéTV Camiseteria | Copa 2026

> **Escopo do documento:** Mapeamento completo de origens e mídias que serão analisadas pela agência de performance. Contempla 20 combinações de canal × formato — orgânico e pago. A agência analisa e reporta; não cria conteúdo orgânico nem gerencia comunidades.

> **Framework de análise:** Toda chamada publicada em qualquer canal é uma unidade de análise rastreável até a loja CazéTV no Mercado Livre. O funil universal (Exposição → CTR → Sessões ML → Conversão), o padrão de UTMs, a lógica de QR codes em lives e o loop de otimização estão detalhados no documento **`framework_analise_por_chamada.md`**.

---

## Visão Geral dos Canais

| # | Canal | Mídia / Formato | Tipo | Timing de análise | Ação em tempo real? |
|---|---|---|---|---|---|
| 1 | YouTube | Vídeos (chamadas de transmissões) | Orgânico | D+1 / D+7 / D+30 | Não — insight p/ próxima chamada |
| 2 | YouTube | Shorts | Orgânico | D+1 / D+7 | Não |
| 3 | YouTube | **Lives** | Orgânico | ✅ **Real-time + D+1** | Sim — chat, QR code, mensagem fixada |
| 4 | YouTube | Playlists | Orgânico | Semanal | Não — estrutural |
| 5 | YouTube | Posts do canal | Orgânico | D+2 / Semanal | Não |
| 6 | Instagram | Bio | Orgânico | Semanal | Sim — trocar link se CTR baixo |
| 7 | Instagram | **Stories** | Orgânico + Pago | ⚡ Intraday (2–4h) / Diário (pago) | Sim — story de reforço, ajustar link |
| 8 | Instagram | Reels | Orgânico + Pago | D+3 / D+7 / Diário (pago) | Não |
| 9 | Instagram | Posts (feed) | Orgânico + Pago | D+2 / D+7 / Diário (pago) | Parcial — comentar com link |
| 10 | Instagram | Comunidade CazéTV | Orgânico | Semanal | Parcial — nova mensagem de reforço |
| 11 | Instagram | Comunidade Casimiro | Monitoramento | Semanal | Não — canal de terceiro |
| 12 | TikTok | Posts | Orgânico | D+1 / D+7 | Parcial — pinned comment |
| 13 | TikTok | **Vídeos** | Orgânico + Pago | ⚡ Intraday (2–4h) / Diário (pago) | Parcial — pinned comment, repost |
| 14 | TikTok | Stories | Orgânico | D+1 | Não — expira em 24h |
| 15 | TikTok | **Lives** | Orgânico | ✅ **Real-time + D+1** | Sim — CTA verbal, produto em cena |
| 16 | TikTok | TikTok Shop | Orgânico + Pago | Semanal / Diário (pago) | Sim — vitrine, ordem de produtos |
| 17 | Twitter / X | **Tweets** | Orgânico + Pago | ⚡ Intraday (2–4h) / Diário (pago) | Sim — tweet de reforço, fixar tweet |
| 18 | Twitter / X | Enquetes | Orgânico | Ao encerramento + D+1 | Não |
| 19 | WhatsApp | **Comunidade** | Orgânico | ⚡ Intraday (2–4h) | Sim — mensagem de reforço |
| 20 | Threads | Posts | Orgânico | D+3 / D+7 | Parcial — reply com link |

---

## Indicadores de Conversão ML — Universais por Chamada

Além dos indicadores de canal listados em cada seção abaixo, **toda chamada publicada em qualquer das 20 mídias** deve ser analisada no funil de conversão até a loja CazéTV no Mercado Livre. O funil completo, o padrão de UTMs, a estratégia de QR codes e o loop de otimização estão em **`framework_analise_por_chamada.md`**.

Os indicadores abaixo se aplicam universalmente, com o timing específico de cada canal conforme a tabela de visão geral:

| Indicador | Categoria | Como rastrear |
|---|---|---|
| Impressões / Alcance | Exposição | Analytics nativo do canal |
| CTR da chamada (%) | Interesse | Analytics nativo — cliques no link / impressões |
| Cliques absolutos no link / QR scans | Interesse | Analytics nativo + rastreador de QR code |
| Sessões na loja ML (rastreadas) | Acesso | GA4 com UTM por chamada — `utm_content=[id-chamada]` |
| Taxa de drop CTR → Sessão ML (%) | Eficiência | Cliques no canal vs. sessões no GA4 — identifica problemas de link |
| Visualizações de produto na ML | Consideração | ML Analytics / GA4 |
| Add to cart na ML | Consideração | ML Analytics / GA4 |
| Pedidos atribuídos à chamada | Conversão | GA4 + ML Analytics com UTM rastreada |
| Taxa de conversão ML (%) | Conversão | Pedidos / Sessões ML |
| Receita atribuída (R$) | Negócio | Valor dos pedidos com origem na chamada |

> **Nota sobre acessos orgânicos não rastreados:** Uma parte dos acessos à loja ML virá de buscas diretas no próprio Mercado Livre, estimuladas pelas chamadas mas sem link clicado. Medir o volume de acessos orgânicos à loja antes, durante e após cada publicação para capturar o uplift indireto.

---

## YouTube

### 1. YouTube / Vídeos — Chamadas de Transmissões

> **Tipo:** Orgânico | **Granularidade:** Por vídeo (por jogo) | **Ferramenta:** YouTube Studio / YouTube Analytics

Foco principal: avaliar a performance das **chamadas** (título + thumbnail + descrição) dos 104 jogos da Copa transmitidos ao vivo no YouTube. O CTR do thumbnail é o indicador mais sensível à qualidade da chamada.

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Impressões do thumbnail | Alcance | D+1 / Semanal |
| CTR do thumbnail | Eficiência da chamada | D+1 / Semanal |
| Visualizações totais | Consumo | D+1 / D+7 / D+30 |
| Watch time total | Consumo | D+7 / D+30 |
| Duração média de visualização | Consumo | D+7 / D+30 |
| Taxa de retenção (por momento do vídeo) | Consumo | D+7 |
| Espectadores únicos | Alcance | D+7 |
| Inscritos ganhos / perdidos | Audiência | D+7 |
| Likes / Comentários / Compartilhamentos | Engajamento | D+3 / Semanal |
| Origem das visualizações (busca, recomendado, externo) | Alcance | Semanal |
| Cliques em cards e end screens | Conversão | D+7 |

> **Observação:** Comparar CTR entre jogos do Brasil vs. outros jogos — hipótese de que chamadas com Brasil têm CTR 30–50% maior. Cruzar esse dado com o número de impressões para identificar quais thumbnails performam acima da média no contexto da competição.

---

### 2. YouTube / Shorts

> **Tipo:** Orgânico | **Granularidade:** Por Short | **Ferramenta:** YouTube Studio

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Visualizações | Consumo | D+1 / D+7 |
| Impressões na aba de Shorts | Alcance | D+1 / D+7 |
| CTR na aba de Shorts | Eficiência | D+1 / D+7 |
| Taxa de conclusão (completion rate) | Consumo | D+7 |
| Taxa de retenção por segundo | Consumo | D+7 |
| Likes / Comentários / Compartilhamentos | Engajamento | D+3 / Semanal |
| Inscritos ganhos via Short | Audiência | D+7 |
| Cliques no perfil a partir do Short | Conversão | D+7 |

---

### 3. YouTube / Live

> **Tipo:** Orgânico | **Granularidade:** Por live (por jogo) | **Ferramenta:** YouTube Studio / Live Dashboard

A análise da live tem três momentos distintos com indicadores próprios.

**Pré-live — A Chamada**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Impressões da chamada pré-live | Alcance | D-1 (antes do jogo) |
| CTR da chamada pré-live | Eficiência da chamada | D-1 / D+1 |
| Cliques em "Definir lembrete" / notificações enviadas | Audiência | D-1 |

**Durante a Live**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Pico de espectadores simultâneos | Alcance | Real-time |
| Espectadores simultâneos por momento (curva) | Consumo | Real-time / D+1 |
| Espectadores únicos totais | Alcance | Pós-live |
| Watch time durante a transmissão | Consumo | Real-time / D+1 |
| Mensagens no chat por minuto | Engajamento | Real-time |
| Compartilhamentos durante a live | Engajamento | Pós-live |

**Pós-live — VOD**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Visualizações do VOD | Consumo | D+1 / D+7 |
| Watch time do VOD | Consumo | D+7 |
| Taxa de retenção do VOD | Consumo | D+7 |
| Likes / Comentários no VOD | Engajamento | D+3 / Semanal |

> **Observação:** O relatório pós-live de cada jogo deve consolidar os três momentos em um único documento comparativo. Ao longo da Copa, montar um ranking de lives por pico de espectadores e cruzar com o CTR da chamada para identificar padrões.

---

### 4. YouTube / Playlists

> **Tipo:** Orgânico | **Granularidade:** Por playlist | **Ferramenta:** YouTube Analytics (Relatórios → Playlists)

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Playlist starts | Consumo | Semanal |
| Visualizações vindas de playlists | Consumo | Semanal |
| Média de vídeos assistidos por playlist start | Consumo | Semanal |
| Watch time gerado via playlists | Consumo | Semanal / Mensal |
| Taxa de continuidade (avanço para próximo vídeo) | Consumo | Semanal |
| Vídeos com maior taxa de saída na playlist | Eficiência | Mensal |

---

### 5. YouTube / Posts do Canal

> **Tipo:** Orgânico | **Granularidade:** Por post | **Ferramenta:** YouTube Studio (aba Comunidade)

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Impressões | Alcance | D+2 / Semanal |
| Likes | Engajamento | D+2 / Semanal |
| Comentários | Engajamento | D+2 / Semanal |
| Taxa de engajamento (likes + comentários / impressões) | Eficiência | Semanal |
| Cliques em links (se presentes) | Conversão | D+2 / Semanal |

---

## Instagram

### 6. Instagram / Bio

> **Tipo:** Orgânico | **Granularidade:** Conta | **Ferramenta:** Instagram Insights + Linktree / Beacons Analytics

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Visitas ao perfil | Alcance | Semanal |
| Cliques no link da bio | Conversão | Semanal |
| Taxa de conversão perfil → link (cliques / visitas) | Eficiência | Semanal |
| Cliques no botão de DM / e-mail (se configurado) | Conversão | Semanal |
| Evolução de seguidores (net growth) | Audiência | Semanal |

> **Observação:** O link da bio é ponto de entrada ativo para a camiseteria. Cruzar crescimento de visitas ao perfil com publicação de Reels e posts de produto para identificar quais formatos geram mais tráfego para a bio.

---

### 7. Instagram / Stories

> **Tipo:** Orgânico + Pago | **Granularidade:** Por story (orgânico) / Por conjunto de anúncios (pago) | **Ferramenta:** Instagram Insights / Meta Ads Manager

**Orgânico**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Alcance por story | Alcance | D+1 |
| Impressões por story | Alcance | D+1 |
| Taps para frente | Consumo | D+1 |
| Taps para trás | Consumo | D+1 |
| Taxa de saída (swipe away + fechamento) | Eficiência | D+1 |
| Cliques no link (sticker) | Conversão | D+1 |
| Respostas (replies) | Engajamento | D+1 |
| Compartilhamentos | Engajamento | D+1 |

**Pago**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| CPM (custo por mil impressões) | Negócio | Diário |
| CPC (custo por clique) | Negócio | Diário |
| CTR | Eficiência | Diário |
| Frequência | Alcance | Diário |
| Alcance pago | Alcance | Diário |
| Custo por resultado (objetivo da campanha) | Negócio | Diário |
| Conversões atribuídas | Conversão | Diário |

---

### 8. Instagram / Reels

> **Tipo:** Orgânico + Pago | **Granularidade:** Por Reel (orgânico) / Por conjunto de anúncios (pago) | **Ferramenta:** Instagram Insights / Meta Ads Manager

**Orgânico**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Reproduções (plays) | Consumo | D+3 / D+7 |
| Contas alcançadas | Alcance | D+3 / D+7 |
| % de alcance de não-seguidores | Alcance | D+7 |
| Impressões | Alcance | D+3 / D+7 |
| Taxa de conclusão | Consumo | D+7 |
| Likes / Comentários / Compartilhamentos / Salvamentos | Engajamento | D+3 / D+7 |
| Taxa de engajamento | Eficiência | D+7 |
| Visitas ao perfil a partir do Reel | Conversão | D+7 |
| Novos seguidores via Reel | Audiência | D+7 |

**Pago**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| CPM | Negócio | Diário |
| CPV (custo por reprodução) | Negócio | Diário |
| ThruPlay rate (assiste ≥ 15s ou completo) | Consumo | Diário |
| CTR | Eficiência | Diário |
| Conversões / CPA | Conversão | Diário |

---

### 9. Instagram / Posts (Feed)

> **Tipo:** Orgânico + Pago | **Granularidade:** Por post (orgânico) / Por conjunto de anúncios (pago) | **Ferramenta:** Instagram Insights / Meta Ads Manager

**Orgânico**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Alcance | Alcance | D+2 / D+7 |
| Impressões | Alcance | D+2 / D+7 |
| Likes / Comentários / Compartilhamentos / Salvamentos | Engajamento | D+2 / D+7 |
| Taxa de engajamento (total interações / alcance) | Eficiência | D+7 |
| Visitas ao perfil a partir do post | Conversão | D+7 |
| Salvamentos (indicador de intenção de revisita) | Engajamento | D+7 |

**Pago**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| CPM / CPC | Negócio | Diário |
| CTR | Eficiência | Diário |
| Custo por engajamento | Negócio | Diário |
| Alcance pago | Alcance | Diário |
| Conversões / CPA | Conversão | Diário |

---

### 10. Instagram / Comunidade CazéTV

> **Tipo:** Orgânico | **Granularidade:** Por mensagem / Conta | **Ferramenta:** Instagram Insights (aba Comunidade)

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Total de membros | Audiência | Semanal |
| Crescimento líquido de membros | Audiência | Semanal |
| Taxa de abertura / visualização de mensagens | Consumo | Por transmissão + Semanal |
| Reações por mensagem | Engajamento | Por transmissão |
| Respostas por mensagem | Engajamento | Por transmissão |
| Cliques em links por mensagem | Conversão | Por transmissão |
| Taxa de saída (opt-out) | Audiência | Semanal |

---

### 11. Instagram / Comunidade Casimiro

> **Tipo:** Monitoramento externo | **Granularidade:** Por post com menção | **Ferramenta:** BrandWatch + acordo com equipe do Casimiro

> **Nota de acesso:** Canal de terceiro — sem controle editorial. Dados nativos dependem de acordo com a equipe do Casimiro. BrandWatch cobre menções públicas via keyword.

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Volume de menções à camiseteria / CazéTV | Alcance | Semanal |
| Sentimento das menções (positivo / neutro / negativo) | Sentimento | Semanal |
| Engajamento (curtidas + comentários) nos posts com menção | Engajamento | Semanal |
| Alcance estimado dos posts mencionados | Alcance | Semanal |
| Temas recorrentes nos comentários sobre produto | Sentimento | Mensal |

---

## TikTok

### 12. TikTok / Posts

> **Tipo:** Orgânico | **Granularidade:** Por post | **Ferramenta:** TikTok Analytics

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Visualizações | Consumo | D+2 / D+7 |
| Likes / Comentários / Compartilhamentos / Salvamentos | Engajamento | D+2 / D+7 |
| Taxa de engajamento | Eficiência | D+7 |
| Visitas ao perfil a partir do post | Conversão | D+7 |
| Novos seguidores via post | Audiência | D+7 |
| Origem das visualizações (FYP vs. seguidores vs. busca) | Alcance | D+7 |

---

### 13. TikTok / Vídeos

> **Tipo:** Orgânico + Pago | **Granularidade:** Por vídeo (orgânico) / Por campanha (pago) | **Ferramenta:** TikTok Analytics / TikTok Ads Manager

**Orgânico**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Visualizações | Consumo | D+1 / D+7 |
| Watch time médio | Consumo | D+7 |
| Taxa de conclusão | Consumo | D+7 |
| Likes / Comentários / Compartilhamentos / Salvamentos | Engajamento | D+1 / D+7 |
| Alcance via For You Page (FYP) | Alcance | D+7 |
| Origem das visualizações (FYP / busca / perfil / som / seguindo) | Alcance | D+7 |
| Novos seguidores via vídeo | Audiência | D+7 |

**Pago**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| CPM | Negócio | Diário |
| CPV (custo por visualização) | Negócio | Diário |
| ThruPlay rate | Consumo | Diário |
| CTR (para link de destino) | Eficiência | Diário |
| Conversões / CPA | Conversão | Diário |

---

### 14. TikTok / Stories

> **Tipo:** Orgânico | **Granularidade:** Por story | **Ferramenta:** TikTok Analytics

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Visualizações | Consumo | D+1 |
| Taxa de conclusão | Consumo | D+1 |
| Saídas (swipe away) | Eficiência | D+1 |
| Cliques no link (sticker, se disponível) | Conversão | D+1 |
| Respostas (replies) | Engajamento | D+1 |
| Impressões | Alcance | D+1 |

---

### 15. TikTok / Lives

> **Tipo:** Orgânico | **Granularidade:** Por live | **Ferramenta:** TikTok Live Analytics

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Pico de espectadores simultâneos | Alcance | Real-time / Pós-live |
| Total de espectadores únicos | Alcance | Pós-live (D+1) |
| Watch time total da live | Consumo | Pós-live (D+1) |
| Duração média de visualização por espectador | Consumo | Pós-live (D+1) |
| Novos seguidores durante a live | Audiência | Pós-live (D+1) |
| Comentários por minuto (pico de engajamento) | Engajamento | Real-time / Pós-live |
| Compartilhamentos durante a live | Engajamento | Pós-live (D+1) |
| Diamantes recebidos (se ativado) | Negócio | Pós-live (D+1) |

---

### 16. TikTok / TikTok Shop

> **Tipo:** Orgânico + Pago | **Granularidade:** Por produto / Por campanha | **Ferramenta:** TikTok Shop Seller Center / TikTok Ads Manager

> **Nota:** TikTok Shop em expansão no Brasil. Confirmar disponibilidade e ativação antes de incluir no escopo pago.

**Orgânico (Showcase / Vitrine)**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Impressões de produto | Alcance | Semanal |
| CTR do produto (impressão → página) | Eficiência | Semanal |
| Add to cart rate | Conversão | Semanal |
| Taxa de conversão (add to cart → compra) | Conversão | Semanal |
| Receita gerada via TikTok Shop | Negócio | Semanal |
| Volume de devoluções / pedidos cancelados | Negócio | Semanal |
| Avaliações (volume e nota média) | Sentimento | Semanal |

**Pago (Shopping Ads)**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| ROAS (retorno sobre gasto em ads) | Negócio | Diário |
| CPA (custo por aquisição) | Negócio | Diário |
| CTR dos anúncios de shopping | Eficiência | Diário |
| Receita atribuída a anúncios | Negócio | Diário |

---

## Twitter / X

### 17. Twitter / Tweets

> **Tipo:** Orgânico + Pago | **Granularidade:** Por tweet (orgânico) / Por campanha (pago) | **Ferramenta:** X Analytics / X Ads Manager

**Orgânico**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Impressões | Alcance | D+1 / D+3 |
| Engajamentos totais | Engajamento | D+1 / D+3 |
| Taxa de engajamento | Eficiência | D+3 |
| Likes / Retweets / Quote Tweets / Respostas | Engajamento | D+1 / D+3 |
| Cliques em links | Conversão | D+1 / D+3 |
| Cliques no perfil | Conversão | D+3 |
| Bookmarks (salvamentos) | Engajamento | D+3 |

> **Observação:** O Twitter tem ciclo de vida de conteúdo muito curto (< 24h para a maioria dos tweets). A análise de D+3 já captura o pico e a cauda. Monitorar picos de engajamento em dias de jogo — tweets durante transmissões tendem a ter alcance orgânico muito maior.

**Pago**

| Indicador | Categoria | Periodicidade |
|---|---|---|
| CPM / CPC | Negócio | Diário |
| CTR | Eficiência | Diário |
| Engajamentos pagos | Engajamento | Diário |
| Alcance pago | Alcance | Diário |
| Conversões atribuídas | Conversão | Diário |

---

### 18. Twitter / Enquetes

> **Tipo:** Orgânico | **Granularidade:** Por enquete | **Ferramenta:** X Analytics (nativo)

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Impressões | Alcance | Ao encerramento + D+1 |
| Votos totais | Engajamento | Ao encerramento |
| Distribuição de votos (% por opção) | Engajamento | Ao encerramento |
| Taxa de participação (votos / impressões) | Eficiência | Ao encerramento + D+1 |
| Comentários após encerramento | Engajamento | D+1 |
| Retweets / Quote Tweets | Engajamento | D+1 |

> **Observação:** Enquetes funcionam bem em contextos de decisão da torcida (ex.: "Qual seleção vai passar?"). Cruzar taxa de participação com horário de publicação para identificar melhor janela de postagem.

---

## WhatsApp

### 19. WhatsApp / Comunidade

> **Tipo:** Orgânico | **Granularidade:** Por mensagem / Conta | **Ferramenta:** WhatsApp Business (nativo) / Meta Business Suite

> **Nota:** As comunidades do WhatsApp têm métricas mais limitadas que canais de broadcast via API. Avaliar integração com plataforma de disparo (ex.: Notificame, Zenvia) para métricas mais granulares por mensagem.

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Total de membros | Audiência | Semanal |
| Crescimento líquido de membros | Audiência | Semanal |
| Taxa de abertura de mensagens | Consumo | Por transmissão + Semanal |
| Reações por mensagem | Engajamento | Por transmissão |
| Cliques em links por mensagem | Conversão | Por transmissão |
| Taxa de saída (opt-out) | Audiência | Semanal |
| Mensagens enviadas vs. abertas (delivery vs. open rate) | Eficiência | Por transmissão |

---

## Threads

### 20. Threads / Posts

> **Tipo:** Orgânico | **Granularidade:** Por post | **Ferramenta:** Threads Insights (nativo) / Meta Business Suite

> **Nota:** Threads não possui anúncios disponíveis no Brasil (maio/2026). Métricas via integração nativa com Instagram / Meta. Monitorar evolução da plataforma — possível ativação de ads até o início da Copa.

| Indicador | Categoria | Periodicidade |
|---|---|---|
| Visualizações | Consumo | D+3 / D+7 |
| Likes | Engajamento | D+3 / D+7 |
| Respostas | Engajamento | D+3 / D+7 |
| Reposts | Engajamento | D+3 / D+7 |
| Citações (quotes) | Engajamento | D+7 |
| Taxa de engajamento | Eficiência | D+7 |
| Alcance | Alcance | D+7 |
| Visitas ao perfil a partir do post | Conversão | D+7 |

---

## Cadência de Relatórios

| Frequência | Formato | Canais cobertos | Objetivo |
|---|---|---|---|
| **Real-time** (dias de jogo) | Dashboard ao vivo | YouTube Live, YouTube Vídeos (CTR), Twitter, TikTok Live | Monitoramento em tempo real — pico de espectadores, CTR da chamada, trending |
| **Pós-jogo** (D+1) | Relatório por evento | YouTube Live, YouTube Vídeo, Twitter, TikTok Live | Consolidado da performance por jogo da Copa |
| **Diário** | Relatório sintético (pago) | Todos os canais com mídia paga ativa | Controle de budget, CPM, CTR, CPA — acionar otimizações |
| **Semanal** | Relatório analítico | Todos os 20 canais | Performance consolidada + ranking de conteúdos + insights + recomendações |
| **Mensal** | Relatório estratégico | Todos os 20 canais | Revisão de estratégia, benchmarks, recomendações de ajuste de mix de mídia |

---

## Acessos Necessários para Mensuração

| Plataforma | Acesso necessário |
|---|---|
| YouTube | Acesso de visualização ao YouTube Studio (canal CazéTV) |
| Instagram / Meta | Acesso de analista no Meta Business Suite + Meta Ads Manager |
| TikTok | Acesso ao TikTok Analytics (Business Account) + TikTok Ads Manager |
| Twitter / X | Acesso ao X Analytics + X Ads (se pago) |
| WhatsApp | Acesso ao WhatsApp Business ou plataforma de disparo com relatórios |
| Threads | Acesso via Meta Business Suite (integrado ao Instagram) |
| BrandWatch | Licença ativa com keywords configuradas para monitoramento |
| Google Analytics / GA4 | Acesso de visualização + UTMs configuradas para rastreio por canal |

---

*7 de maio de 2026 — Versão 1.0*
