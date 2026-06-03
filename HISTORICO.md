# Histórico do Projeto — LP Ponte Rolante (Astec)

## Sessão 1 — Criação da Landing Page

**Data:** 2026-06-03  
**Base:** LP Talha Elétrica (`../Talha Elétrica/index.html`)  
**Referência:** `ASTEC_LP_DESIGN_BRIEF.md` (seções 4–17)

---

### Arquivos criados

| Arquivo | Descrição |
|---------|-----------|
| `index.html` | LP completa — 10 seções + float WA |
| `assets/css/styles.css` | Design system Astec (idêntico à Talha, comentários atualizados) |
| `assets/js/ui.js` | Interações: navbar scroll, menu mobile, FAQ accordion, scroll reveal, animação solution-cards, active nav |

---

### Estrutura de seções

| # | ID | Nome | Status |
|---|-----|------|--------|
| 1 | `#navbar` | Navbar | Reutilizado — links e WA text atualizados para PR |
| 2 | `#hero` | Hero | Reescrito — novo badge, headline, parágrafo, CTAs e badges da foto |
| 3 | `#solucoes` | Soluções | **Novo** — substitui catálogo e-commerce (6 cards, sem filtros) |
| 4 | `#manutencao` | Manutenção | Copy ajustado ("talha" → "ponte rolante") |
| 5 | `#diferenciais` | Por que Astec | Reutilizado na íntegra |
| 6 | `#como-funciona` | Como Funciona | Passo 1 reescrito com parâmetros de PR |
| 7 | `#prova-social` | Prova Social | Selo atualizado para "+30 anos de projetos" |
| 8 | `#faq` | FAQ | 7 perguntas específicas de PR |
| 9 | `#orcamento` | Contato | Links WA atualizados |
| 10 | `footer` | Footer | Coluna "Modelos" → "Soluções" com 6 tipos |
| — | `#whatsapp-float` | Botão WA flutuante | Links WA atualizados |

---

### Hero — alterações específicas

| Elemento | Valor aplicado |
|----------|---------------|
| Badge pulsante | "Especialistas em Pontes Rolantes no Rio Grande do Sul" |
| Headline L1 | "Pontes" |
| Headline L2 | "Rolantes" |
| Headline L3 | "e Pórticos para sua Planta" |
| CTA primário | "Ver Soluções" → `#solucoes` |
| CTA secundário | "Cotar Ponte Rolante" → WhatsApp |
| Stat bar 3º card | "NR / 11 e NR-12" |
| Foto hero | `fotos/Fabricacao_Pontes_Rolantes.jpeg` |
| Capacidade overlay | "1 t – 80 t+" |
| Badges foto | Monovia · Dupla Viga · Pórtico |
| Badges header | NR-11 · RS |

---

### Seção Soluções — 6 cards

| ID | Nome | Capacidade | Cor destaque |
|----|------|-----------|--------------|
| PR-MONO | Ponte Rolante Monovia | 1 t – 10 t | Azul (`#004EA2`) |
| PR-DV | Ponte Rolante Dupla Viga | 10 t – 50 t+ | Azul escuro (`#003872`) + badge "Cargas Pesadas" |
| PO-MONO | Pórtico Monovia | 2 t – 20 t | Verde (`#16A34A`) |
| PO-DV | Pórtico Dupla Viga | 10 t – 80 t+ | Laranja (`#F97316`) |
| PR-SEMI | Semi-Pórtico | 2 t – 30 t | Azul claro (`#4267AA`) |
| PR-ESP | Projetos Especiais | Sob consulta | Laranja + badge "EXCLUSIVO ASTEC" |

---

### Fotos utilizadas

| Arquivo | Seção |
|---------|-------|
| `fotos/Fabricacao_Pontes_Rolantes.jpeg` | Hero — painel direito |
| `fotos/Desmontagem_Equipamentos.jpeg` | Manutenção Corretiva (card foto) |
| `fotos/Montagem_Desmontagem_Equipamentos (1).jpeg` | Retrofit / Modernização (card foto) |
| `fotos/Parque_Fabril.jpeg` | Disponível — não utilizada (reserva para futuras seções) |

---

### FAQ — 7 perguntas de Ponte Rolante

1. Qual a diferença entre ponte rolante monovia e dupla viga?
2. Qual a diferença entre ponte rolante e pórtico?
3. Vocês atendem manutenção de pontes de outras marcas? (Demag, Konecranes, Munck…)
4. A NR-11 é obrigatória para pontes rolantes?
5. Como é feito o dimensionamento de uma ponte rolante?
6. Vocês fabricam pontes rolantes ou apenas instalam e mantêm?
7. Em quais regiões a Astec atende?

---

### Ajustes posteriores (mesma sessão)

| Item | Alteração |
|------|-----------|
| **Stepper "Como Funciona"** | Alinhamento horizontal corrigido: container `items-start`, conectores com `self-start mt-8` para coincidir com o centro dos ícones de 64px |

---

### Publicação — GitHub Pages

| Item | Valor |
|------|-------|
| Repositório | `Stanleics/astec-landing-page-portico` |
| URL online | https://stanleics.github.io/astec-landing-page-portico |
| Branch | `main` |
| Path Pages | `/` (raiz) |

---

### Pendências / Confirmações com o cliente

- [ ] Confirmar quais soluções a Astec efetivamente fornece (PR-MONO, PR-DV, PO-MONO, PO-DV, PR-SEMI, PR-ESP)
- [ ] Confirmar capacidades máximas reais por tipo
- [ ] Confirmar se fabricam sob medida ou atuam como integradores (FAQ item 6)
- [ ] Validar respostas do FAQ (prazos, capacidades, NR-11)
- [ ] Substituir `fotos/Parque_Fabril.jpeg` se quiser usá-la em alguma seção
- [ ] Adicionar foto adicional de ponte rolante em operação quando o cliente enviar
- [ ] Atualizar selo da Prova Social com número real de pontes instaladas

---

### Stack técnica

```
HTML5 + Tailwind CSS Play CDN + JavaScript Vanilla
Sem framework, sem bundler — arquivo index.html único
```
