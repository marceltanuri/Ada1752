# Avaliação Coding Tank – Desafio "Marketplace Priority Sorter" (MPS)

---

## 1. Instruções gerais

1. Formem **grupos de 4 a 5 pessoas**. Cada integrante deve ter um papel claro (facilitador(a), analista de algoritmos, designer de diagramas, relator/a, etc.) ou assumir tarefas específicas a partir do backlog que o grupo definir.
2. O trabalho **não exige código**. A entrega consiste em dois artefatos:
    * **Documento PDF (máximo 2 páginas)**, elaborado seguindo o template descrito na seção 3 deste documento. O documento pode ter formato de *canvas*; esclarecemos que o termo "canvas" aqui **não** se refere à ferramenta Canva.com: significa simplesmente um documento de uma ou duas páginas que organiza a solução em blocos. Podem produzi-lo na ferramenta que preferirem (Google Docs, Word, Miro, Notion, Slack canvas, etc.) e exportá-lo em PDF.
    * **Apresentação ao vivo** do grupo no Dia 3 (ver item 1.4).
3. **Entrega dos arquivos**: o envio é feito exclusivamente pelo **formulário oficial de entrega** (link e campos detalhados ao final deste documento). **Não** serão aceitas entregas por e-mail nem pelo LMS. O prazo final é o **encerramento do Dia 2 (23h59, horário de Brasília)**. Recomenda-se manter também uma cópia de backup em um repositório próprio (Google Drive, GitHub, etc.).
4. **Apresentação do Dia 3**:
    * 15 minutos de exposição + 10 minutos de perguntas por grupo.
    * A apresentação deve ser feita ao vivo e exclusivamente pelos integrantes do grupo. Não serão aceitos vídeos pré-gravados, slides com narração pré-gravada nem qualquer outro formato assíncrono.
    * Não é obrigatório que todos os integrantes falem o mesmo tempo, mas o grupo deve deixar clara a **participação e o domínio de cada membro** sobre a solução apresentada. Algumas formas de fazer isso:
        * Distribuir a exposição entre duas ou três vozes e deixar o Q&A para os demais integrantes.
        * Iniciar a apresentação com uma breve menção de "quem fez o quê" (modelagem, diagrama, métricas, redação, etc.).
        * Garantir que, durante o Q&A, as perguntas sejam respondidas de forma distribuída — não sempre pela mesma pessoa.
        * Incluir, no encerramento, uma fala curta (1–2 frases) de cada integrante que não tenha exposto, explicando sua contribuição ao trabalho.
        * Usar dinâmicas de revezamento (pair-presenting): uma pessoa explica o "o quê" e outra o "porquê" ou o "como".
    * O suporte visual (slides, documento canvas na tela, diagramas, etc.) é de formato livre, desde que seja legível e acessível.
    * Se algum integrante precisar de algum ajuste de acessibilidade (alto contraste, legendas ao vivo, tempo extra, etc.), deve comunicar aos instrutores antes do início da sessão.
5. O uso de IA generativa é permitido e incentivado, desde que o grupo **cite explicitamente** como e quando a ferramenta foi utilizada e demonstre compreensão própria da solução.

> **Pontuação total: 20 pt** (ver rubrica na seção 4.2). Cada eixo tem peso igual, independentemente do número de artefatos produzidos.

---

## 2. Cenário fictício: Marketplace Priority Sorter (MPS)

O *VelozMart*, grande empresa de logística e varejo da América Latina, lançou uma feature que mostra em tempo real uma lista de **pedidos** aguardando expedição. O objetivo é exibir os pedidos na **ordem ótima** para minimizar atrasos e custos logísticos.

### Elementos do problema

* Cada pedido possui:

    * *priorityScore* (0–100) calculado por IA com base em distância, SLA, valor do item e reputação do vendedor.
    * *dispatchWindow* (minutos restantes até prazo expirar).
    * *sizeCategory* (P, M, G) que impacta espaço na doca de embalagem.
* O time de logística pediu um **protótipo conceitual** que responda:

    1. Como **ordenar** pedidos considerando múltiplos critérios?
    2. Como re‑**enfileirar** pedidos à medida que novos chegam ou prazos mudam?
    3. Quais métricas comprovam que a estratégia é melhor que uma ordenação simples por tempo?

> Existem diversas estratégias válidas: peso composto (priorityScore × 1/dispatchWindow), duas filas (urgentes vs. normais), heap multi‑chave, algoritmo de aproximação de scheduling, etc. A escolha é livre, desde que fundamentada.

### Requisitos mínimos da solução

A solução entregue deve conter **exatamente as cinco seções** descritas no template (seção 3 deste documento):

1. **Problema** — resumo do cenário e dados de contexto.
2. **Algoritmo / Estrutura** — nome, motivação e breve pseudocódigo ou descrição textual do funcionamento.
3. **Diagrama** — imagem autoexplicativa (heap, fluxo, gráfico de Gantt, etc.) que ilustre inclusão, remoção e re-priorização; com legenda e alto contraste.
4. **Trade-offs** — pelo menos 3 prós e 3 contras da escolha, com justificativa.
5. **Próximos passos** — ideias futuras de evolução.

Itens bônus (opcionais, não obrigatórios): análise Big O, comparação entre duas abordagens, proposta de teste A/B ou simulação, discussão de acessibilidade na UI.

---

## 3. Template de entrega (documento canvas em PDF)

O documento entregue deve seguir **exatamente esta estrutura**, uma seção após a outra, em um PDF de **no máximo 2 páginas**:

<table>
  <tr>
    <th>Seção</th>
    <th>Guia de conteúdo</th>
  </tr>
  <tr>
    <td><strong>Problema</strong></td>
    <td>Situação real resumida em 3–4 linhas; dados de contexto relevantes.</td>
  </tr>
  <tr>
    <td><strong>Algoritmo / Estrutura</strong></td>
    <td>Nome, motivação da escolha e breve pseudocódigo ou descrição textual.</td>
  </tr>
  <tr>
    <td><strong>Diagrama</strong></td>
    <td>Imagem autoexplicativa. Use legenda e alto contraste.</td>
  </tr>
  <tr>
    <td><strong>Trade‑offs</strong></td>
    <td>3 prós e 3 contras; justificativa da escolha.</td>
  </tr>
  <tr>
    <td><strong>Próximos passos</strong></td>
    <td>Ideias futuras (ex.: incorporar aprendizagem online).</td>
  </tr>
</table>

> Lembrete: "canvas" significa um documento de uma ou duas páginas organizado em blocos. **Não tem relação com a ferramenta Canva.com.** Podem produzi-lo em qualquer ferramenta (Google Docs, Word, Miro, Notion, Slack canvas, etc.) e exportá-lo em PDF.

