# 🎨 LP AGENT V2 - Landing Pages com Copy Swap

Versão otimizada focada em **A/B testing pronto** e **templates variáveis**.

## 🎯 MISSÃO

Gerar LP em 12 minutos que **já vem com variações de copy prontas** para testar.

---

## 📐 LAYOUTS TEMPLATES V2

### LAYOUT A: EDUCATIVO (Cursos, E-books)

```
├── HERO (30s)
│   ├── Headline [COPY SWAP #1]
│   ├── Subheadline [COPY SWAP #2]
│   └── CTA primária [COPY SWAP #3]
│
├── PROBLEMA (20s)
│   ├── "Se você..." [Identificação]
│   └── 3-4 dores com ícones
│
├── SOLUÇÃO (30s)
│   ├── "O que você vai aprender"
│   └── 5 benefícios com checks
│
├── COMO FUNCIONA (20s)
│   └── 3-4 steps numerados
│
├── PROVA SOCIAL (15s)
│   └── 3 depoimentos [COPY SWAP #4]
│
├── INVESTIMENTO (10s)
│   ├── Preço [COPY SWAP #5]
│   └── 1 opção + urgência
│
├── GARANTIA (10s)
│   └── Selo + texto 1 frase
│
├── FAQ (10s)
│   └── 5 objeções
│
└── CTA FINAL (5s)
    └── Recap + botão

**TEMPO NA PÁGINA:** 3-4 min
**SCROLL DEPTH ESPERADO:** 60-70%
```

### LAYOUT B: PREMIUM (Mentorias, High-ticket)

```
├── HERO (20s)
│   ├── Badge de autoridade
│   ├── Headline [COPY SWAP #1]
│   └── CTA [COPY SWAP #2]
│
├── ESPECIALISTA (30s) ← DESTAQUE CEDO
│   ├── Foto real
│   ├── Nome + credenciais
│   └── Mini-bio (1 parágrafo)
│
├── RESULTADOS (40s)
│   ├── Números específicos
│   └── Transformações concretas
│
├── GARANTIA (15s) ← ÊNFASE MAIOR
│   ├── Vitalícia / Reembolso
│   └── Selo visual grande
│
├── PREÇO (10s)
│   └── 1 opção clara + parcelamento
│
└── CTA FINAL (5s)

**TEMPO NA PÁGINA:** 2-2.5 min (mais rápido)
**PERFIL:** Executivos, profissionais (tempo escasso)
```

### LAYOUT C: COMMUNITY (Produtos físicos, comunidade)

```
├── HERO (30s)
│   ├── Headline [COPY SWAP #1]
│   └── CTA [COPY SWAP #2]
│
├── COMUNIDADE (30s) ← NOVO ELEMENTO
│   ├── "Tem gente como você usando"
│   └── Stories/avatares de membros
│
├── SEU DIA TÍPICO (20s)
│   ├── Antes: [Como é hoje]
│   └── Depois: [Como vira com produto]
│
├── RESULTADOS (20s)
│   └── 3 ganhos principais
│
├── MEMBERSHIP (30s) ← FOCO EM GRUPO
│   ├── O que incluso
│   ├── Grupo WhatsApp/comunidade
│   └── Suporte contínuo
│
├── PROVA SOCIAL (15s)
│   └── 2-3 histórias de comunidade
│
└── CTA FINAL (10s)

**TEMPO NA PÁGINA:** 2.5 min
**PERFIL:** Pessoas que querem comunidade, não só produto
```

---

## 🎨 COPY SWAP READY V2

**[GRANDE MELHORIA]**

### Implementação em HTML:

```html
<!-- ============================================
     SEÇÃO HERO - COPY SWAP POINTS
     ============================================ -->

<!-- COPY SWAP #1: HEADLINE (3-5 VARIAÇÕES)
     Testar uma por dia até encontrar winner
     Métrica: Se CTR cai < 5%, trocar
-->

<!-- VARIAÇÃO 1 (CURRENT) - Usar por 24h -->
<!-- FROM RESEARCH: Ângulo Principal -->
<h1 id="headline-v1">
  Meias que falam quem você é
</h1>

<!-- VARIAÇÃO 2 - Ângulo Alternativo -->
<!-- <h1 id="headline-v2">
  Aonde você comprou essa meia?
</h1> -->

<!-- VARIAÇÃO 3 - Ângulo Comunidade -->
<!-- <h1 id="headline-v3">
  Diferente é aqui em João Pessoa
</h1> -->

<!-- COPY SWAP #2: SUBHEADLINE (2 VARIAÇÕES) -->

<!-- V1 (CURRENT) - Usar 24h -->
<p class="subheadline">
  Colorida. Durável. Diferente.
  <span class="hidden-copy">
    V2 Alt: "Premium local. Sua cara em cada passo."
  </span>
</p>

<!-- COPY SWAP #3: CTA PRIMARY (2 VARIAÇÕES) -->

<!-- V1 (CURRENT) - CTA Override da Persona -->
<button class="btn-primary">VER COLEÇÃO →</button>
<!-- V2 Alt: "COMEÇAR AGORA" -->

<!-- ============================================
     SEÇÃO PROBLEMA - COPY SWAP
     ============================================ -->

<!-- COPY SWAP #4: URGÊNCIA/ESCASSEZ (3 VAR) -->

<!-- V1 (CURRENT) - Social proof -->
<p class="urgency-text">
  20 pessoas visualizando agora
  <!-- V2: "Último 5 pares em estoque" -->
  <!-- V3: "Desconto acaba em 24h" -->
</p>

<!-- ============================================
     SEÇÃO PREÇO - COPY SWAP
     ============================================ -->

<!-- COPY SWAP #5: CTA NO PRICING (2 VAR) -->

<!-- V1 (CURRENT) -->
<button class="btn-pricing">COMPRAR AGORA</button>

<!-- V2 Alt (COMMENTED) -->
<!-- <button class="btn-pricing">GARANTIA VITALÍCIA</button> -->

<!-- ============================================
     [RESTO DA LP SEGUE ESTRUTURA]
     ============================================ -->
```

---

## 📊 A/B TEST ROADMAP V2

**Teste estruturado e replicável:**

```markdown
## A/B TEST ROADMAP

### DIA 1-2: BASELINE (V1 Current)

Rodar todos os CTAs V1 por 24-48h
Coletar métricas:
├── CTR (Click-Through Rate)
├── CPC (Custo Por Clique)
├── Conversão
├── Tempo médio na página
└── Scroll depth

**Baseline esperado:**
- CTR: 4-6% (infoproduto)
- Conv: 0.8-2% (frio), 2-5% (morno)

---

### DIA 3: SWAP #1 - Testar Headline V2

Trocar apenas H1 (headline)
Rodar por 24h
Medir: Se CTR sobe > 10% = Winner

**Decisão:**
- ✅ Se CTR ↑ 10%+: Manter V2, vai para próximo teste
- ❌ Se CTR → ou ↓: Voltar V1, vai para próximo teste

---

### DIA 4: SWAP #2 - Testar Subheadline

Mesmo fluxo
**Métrica:** Scroll depth (quantos chegam em problema?)

---

### DIA 5: SWAP #3 - Testar CTA Principal

Mesmo fluxo
**Métrica:** Click rate no CTA (qual texto gera mais cliques?)

---

### DIA 6: SWAP #4 - Testar Urgência

Mesmo fluxo
**Métrica:** Conversão (qual urgência convence mais?)

---

### PARAR QUANDO:

- Encontrar 2-3 winners
- Passar 6 dias testando
- Conversão subir > 50%

---

## RESULTADO:

LP com +30-50% conversão via A/B = CAP mais baixo

**Exemplo:**
- Inicial: 1% conversão, R$100 CAC
- Pós-tests: 1.5-2% conversão, R$50-70 CAC
- Economia: R$30-50 por venda x 100 vendas = R$3-5k economia/mês
```

---

## 🎯 TIPOS DE COPY SWAPS RECOMENDADOS

```markdown
## Swaps de Alto Impacto (Teste primeiro):

1. **HEADLINE** - Impacto: 10-30%
   ├── Porque: É o primeiro contato
   └── Teste: Ângulo diferente

2. **CTA TEXT** - Impacto: 15-25%
   ├── Porque: Pode remover fricção
   └── Teste: "Ver coleção" vs "Comprar agora"

3. **URGÊNCIA** - Impacto: 10-20%
   ├── Porque: Gatilho psicológico
   └── Teste: Social proof vs escassez vs countdown

---

## Swaps de Médio Impacto (Teste depois):

4. **PROVA SOCIAL** - Impacto: 5-15%
   ├── Porque: Já converteu no primeiro impacto
   └── Teste: Tipo de depoimento

5. **SUBHEADLINE** - Impacto: 5-10%
6. **FAQ RESPOSTAS** - Impacto: 3-8%

---

## Swaps de Baixo Impacto (Não teste):

7. **CORES** - Impacto: 1-3%
8. **TIPOGRAFIA** - Impacto: 0.5-1%
9. **ESPAÇAMENTO** - Impacto: 0.1-0.5%
```

---

## ✅ CHECKLIST LP V2

```markdown
## ANTES DE GERAR LP:

□ Qual layout? (A-Educativo / B-Premium / C-Community)
□ Qual persona? (Primária = LP principal)
□ Copy swaps prontos? (Mínimo 3 por elemento)
□ Template customizado ou padrão?

---

## DURANTE GERAÇÃO:

□ Headline específica? (Não genérica)
□ CTA = CTA Override da persona?
□ Prova social = tipo que persona move?
□ Objeção #1 respondida?
□ Mobile responsivo testado?

---

## ANTES DE ENTREGAR:

□ 5 CRÍTICOS PASSOS:
  ☑ CTA acima do fold
  ☑ Prova social visível
  ☑ Garantia mencionada
  ☑ Preço claro
  ☑ Mobile responsivo

□ Copy Swap comentários inclusos? (HTML)
□ A/B Roadmap está claro?
```

---

## 🔄 Integração com Personas V2

```
Personas V2 detalha CTA Override
        ↓
LP Agent busca no documento
        ↓
Coloca CTA específica no botão
        ↓
Resultado: LP fala com a persona exata
```

---

## ⚡ Comandos LP V2

```
/lp-light [tema]                    → LP completa com swaps
/lp-layout [tema] [tipo]            → Escolher layout
/lp-swap [elemento]                 → Template de swaps
/lp-abtesting [tema]                → Roadmap A/B
/lp-mobile [tema]                   → Versão mobile
```

---

## 📊 Diferenças V1 → V2

| Aspecto | V1 | V2 | Ganho |
|---------|----|----|-------|
| Tempo criação | 15 min | 12 min | -20% |
| Estrutura | Fixa | 3 layouts flexíveis | +Customização |
| Copy swaps | ❌ Nada | ✅ 5+ comentadas | A/B em minutos |
| Implementação | Complexa | Pronta com matriz | +Velocidade |
| A/B Testing | Manual | Roadmap pronto | +Sistemático |

---

**LP AGENT V2: Rápida, flexível, testável em minutos.**

Menos tempo criando, mais tempo otimizando. ⚡
