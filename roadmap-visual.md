# Roadmap Visual - BRPF 2025

## 🗺️ Roadmap Interativo em Mermaid

```mermaid
gantt
    title BRPF 2025 - Brasil Pump Festival Roadmap
    dateFormat  YYYY-MM-DD
    axisFormat  %d/%m

    section 🚨 FASE CRÍTICA
    Reunião Orçamento           :crit, orcamento, 2025-08-12, 2025-08-15
    Definir Categorias          :crit, categorias, 2025-08-16, 2025-08-18
    Negociar Locais            :crit, locais, 2025-08-20, 2025-08-22
    DECISÃO LOCAL              :milestone, decisao, 2025-08-25, 0d
    Contratar Fornecedores     :crit, fornecedores, 2025-08-26, 2025-08-31

    section 📋 PLANEJAMENTO
    Criar Regras               :regras, after categorias, 5d
    Listas de Músicas          :musicas, after regras, 3d
    Equipe de Som              :som, after decisao, 7d
    Transporte Máquinas        :transporte, after decisao, 7d
    Social Media/Video         :midia, after decisao, 10d

    section 🎨 PRODUÇÃO
    Material Divulgação        :divulgacao, 2025-09-15, 7d
    Teste Equipamentos         :testes, 2025-09-17, 3d
    Reunião Equipe             :reuniao, 2025-09-19, 1d
    Campanha Marketing         :campanha, 2025-09-22, 5d
    Redes Sociais              :redes, 2025-09-24, 2d
    Valores Inscrição          :valores, 2025-09-26, 2d

    section 🎯 EXECUÇÃO
    Materiais Gráficos         :graficos, 2025-09-30, 3d
    ABERTURA INSCRIÇÕES        :milestone, inscricoes, 2025-10-06, 0d
    Divulgação Intensiva       :intensa, 2025-10-08, 14d
    Contratar Foto/Vídeo       :foto, 2025-10-13, 3d
    Teste Completo             :teste-completo, 2025-10-15, 2d
    Conteúdo Promocional       :promocional, 2025-10-20, 7d
    Listas Públicas            :listas-publicas, 2025-10-22, 2d

    section 🏁 FINALIZAÇÃO
    FECHAMENTO INSCRIÇÕES      :milestone, fechamento, 2025-11-03, 0d
    Sorteio Brackets           :brackets, 2025-11-05, 2d
    Divulgar Brackets          :div-brackets, 2025-11-07, 1d
    Transporte Setup           :setup-transporte, 2025-11-10, 2d
    Setup Completo             :setup, 2025-11-12, 2d
    Teste Final                :teste-final, 2025-11-14, 1d
    EVENTO BRPF 2025           :milestone, evento, 2025-11-22, 2d
```

## 🎯 Marcos Críticos e Dependências

```mermaid
flowchart TD
    A[📅 10/08 - Início Planejamento] --> B{💰 15/08 - Orçamento Definido?}
    B -->|Sim| C[🏢 18/08 - Definir Categorias]
    B -->|Não| D[❌ Risco Alto - Revisar Viabilidade]
    
    C --> E[🤝 20-22/08 - Negociar Locais]
    E --> F{🏆 25/08 - DECISÃO LOCAL}
    
    F -->|Login R$0| G[📊 Cenário Conservador<br/>4 Categorias<br/>60-80 pessoas]
    F -->|Ksquare R$2.900| H[🚀 Cenário Ambicioso<br/>6 Categorias<br/>100+ pessoas]
    
    G --> I[📋 Setembro - Estruturação]
    H --> I
    
    I --> J[🎨 Outubro - Produção e Marketing]
    J --> K[📝 06/10 - Abertura Inscrições]
    K --> L{📊 Inscrições Suficientes?}
    
    L -->|Sim| M[🏁 Novembro - Finalização]
    L -->|Não| N[⚠️ Plano Contingência]
    
    M --> O[🎉 22-23/11 - EVENTO BRPF]
    
    style F fill:#ff6b6b,stroke:#333,stroke-width:3px
    style K fill:#4ecdc4,stroke:#333,stroke-width:2px
    style O fill:#45b7d1,stroke:#333,stroke-width:3px
```

## 📊 Timeline de Riscos e Contingências

```mermaid
timeline
    title Pontos Críticos de Decisão
    
    section Agosto
        15/08 : Orçamento
              : Se não definido = RISCO ALTO
        
        25/08 : Local
              : DECISÃO IRREVERSÍVEL
              : Afeta todo cronograma
    
    section Setembro
        A definir : Fornecedores
                  : Item a ser trabalhado futuramente
        
        26/09 : Preços
              : Define viabilidade financeira
    
    section Outubro
        06/10 : Inscrições
              : Início da receita
        
        25/10 : Cancelamento
              : Último ponto de cancelamento
    
    section Novembro
        03/11 : Fechamento
              : Define sucesso/fracasso
        
        22/11 : EVENTO
              : Execução final
```

## 🎮 Fluxo de Categorias por Local

```mermaid
flowchart LR
    subgraph "🏢 LOGIN - Cenário Conservador"
        L1[Speed Pró M] --> L2[Speed Pró F]
        L2 --> L3[Co-op]
        L3 --> L4[Freestyle]
        L4 --> LT[⏱️ 8-9 horas<br/>60-80 pessoas]
    end
    
    subgraph "🏢 KSQUARE - Cenário Ambicioso"
        K1[Speed Pró M] --> K2[Speed Pró F]
        K2 --> K3[Speed Iniciante]
        K3 --> K4[Speed Intermediário]
        K4 --> K5[Co-op]
        K5 --> K6[Freestyle]
        K6 --> KT[⏱️ 12-13 horas<br/>100+ pessoas<br/>2 dias]
    end
    
    DECISAO{25/08 - Decisão Local} --> LOGIN
    DECISAO --> KSQUARE
    
    LOGIN --> L1
    KSQUARE --> K1
```

## 💰 Análise Financeira Visual

```mermaid
flowchart TD
    subgraph "💰 RECEITAS"
        R1[50 Inscrições x R$100 = R$5.000]
        R2[70 Inscrições x R$100 = R$7.000]
        R3[100 Inscrições x R$100 = R$10.000]
    end
    
    subgraph "🏢 CENÁRIO LOGIN"
        LC[Custos Totais: R$3.600]
        LC1[Equipamentos: R$1.500]
        LC2[Transporte: R$1.000]
        LC3[Pessoal: R$800]
        LC4[Diversos: R$300]
        LC5[Local: R$0]
        
        LC1 --> LC
        LC2 --> LC
        LC3 --> LC
        LC4 --> LC
        LC5 --> LC
    end
    
    subgraph "🏢 CENÁRIO KSQUARE"
        KC[Custos Totais: R$6.500]
        KC1[Local: R$2.500]
        KC2[Som: R$400]
        KC3[Equipamentos: R$1.500]
        KC4[Transporte: R$1.000]
        KC5[Pessoal: R$800]
        KC6[Diversos: R$300]
        
        KC1 --> KC
        KC2 --> KC
        KC3 --> KC
        KC4 --> KC
        KC5 --> KC
        KC6 --> KC
    end
    
    subgraph "📊 RESULTADOS"
        RL1[Login 50p: R$1.400 lucro]
        RL2[Login 70p: R$3.400 lucro]
        RK1[Ksquare 70p: R$500 lucro]
        RK2[Ksquare 100p: R$3.500 lucro]
    end
    
    R1 --> RL1
    R2 --> RL2
    R2 --> RK1
    R3 --> RK2
    
    style RL1 fill:#90EE90
    style RL2 fill:#32CD32
    style RK1 fill:#FFD700
    style RK2 fill:#32CD32
```

## 🎯 Matriz de Risco vs Retorno

```mermaid
quadrantChart
    title Análise de Cenários - Risco vs Retorno
    x-axis Baixo Risco --> Alto Risco
    y-axis Baixo Retorno --> Alto Retorno
    
    quadrant-1 Alto Retorno / Alto Risco
    quadrant-2 Alto Retorno / Baixo Risco
    quadrant-3 Baixo Retorno / Baixo Risco
    quadrant-4 Baixo Retorno / Alto Risco
    
    Login 50p: [0.2, 0.3]
    Login 70p: [0.3, 0.7]
    Ksquare 70p: [0.7, 0.1]
    Ksquare 100p: [0.8, 0.8]
```

## 📈 Cronograma de Participantes

```mermaid
xychart-beta
    title "Projeção de Inscrições por Mês"
    x-axis [Out-Sem1, Out-Sem2, Out-Sem3, Out-Sem4, Nov-Sem1]
    y-axis "Participantes" 0 --> 100
    bar [10, 25, 45, 65, 80]
    line [15, 30, 50, 70, 85]
```

## 🔄 Estados do Projeto

```mermaid
stateDiagram-v2
    [*] --> Planejamento
    Planejamento --> Decisao_Local: 25/08
    
    Decisao_Local --> Login_Escolhido: Custo Zero
    Decisao_Local --> Ksquare_Escolhido: Maior Potencial
    
    Login_Escolhido --> Estruturacao: 4 Categorias
    Ksquare_Escolhido --> Estruturacao: 6 Categorias
    
    Estruturacao --> Producao: Set/2025
    Producao --> Inscricoes: 06/10
    
    Inscricoes --> Suficientes: >50 pessoas
    Inscricoes --> Insuficientes: <40 pessoas
    
    Suficientes --> Finalizacao
    Insuficientes --> Contingencia
    
    Contingencia --> Adiamento
    Contingencia --> Cancelamento
    
    Finalizacao --> Evento: 22-23/11
    Evento --> [*]
```

---

## 🛠️ Como Usar Este Roadmap

### Visualização Online
1. Copie qualquer código Mermaid acima
2. Cole em [mermaid.live](https://mermaid.live)
3. Visualize e exporte como PNG/SVG

### Integração com Documentação
- Os diagramas são renderizados automaticamente no GitHub
- Compatível com GitLab, Notion, e outras plataformas
- Pode ser integrado em apresentações PowerPoint/Google Slides

### Atualizações Dinâmicas
- Modifique as datas conforme necessário
- Adicione novos marcos ou tarefas
- Ajuste as dependências conforme o projeto evolui

### Alternativas de Visualização
Se preferir outras ferramentas além do Mermaid:
- **Lucidchart**: Para diagramas mais elaborados
- **Draw.io**: Gratuito e integrado ao Google Drive
- **Microsoft Project**: Para cronogramas detalhados
- **Trello/Notion**: Para acompanhamento de tarefas

---

## 📅 NOTA SOBRE DATAS ALTERNATIVAS

**Data Preferencial:** 22-23 de novembro de 2025 (aproveitando feriado de 20/11)

**Datas Alternativas para Negociação:**
- **Plano B:** 29-30 de novembro ou 6-7 de dezembro
- **Plano C:** 15-16 de novembro ou 13-14 de dezembro

Todos os diagramas acima refletem o cronograma baseado na data preferencial. Caso seja necessário usar uma data alternativa, os marcos e prazos serão ajustados proporcionalmente.

---

*Roadmap criado em: 08 de dezembro de 2025*  
*Baseado no planejamento completo do BRPF 2025*  
*Atualizado com datas alternativas em: 08 de dezembro de 2025*
