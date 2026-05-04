# FinançaFácil - Especificações Técnicas do Design System

## 📐 Layout Base

### Dimensões da Tela
- **Dispositivo:** iPhone 14 Pro
- **Largura:** 390px
- **Altura:** 844px
- **Proporção:** 9:19.5

### Grid e Espaçamento
- **Margem lateral:** 16px (ambos os lados)
- **Largura do conteúdo:** 358px (390 - 32)
- **Unidade base de espaçamento:** 8px
- **Espaçamentos permitidos:** 8px, 16px, 24px, 32px, 40px, 48px

---

## 🎨 Sistema de Cores

### Cores Primárias

```
Primary/Green
HEX: #27AE60
RGB: 39, 174, 96
Uso: Botões principais, receitas, saldo positivo, ícones ativos
```

```
Danger/Red
HEX: #E74C3C
RGB: 231, 76, 60
Uso: Despesas, alertas, ações destrutivas, saldo negativo
```

```
Info/Blue
HEX: #3498DB
RGB: 52, 152, 219
Uso: Links, elementos informativos, gráficos, destaques
```

### Cores Neutras

```
Text/Dark
HEX: #2C3E50
RGB: 44, 62, 80
Uso: Textos principais, títulos, conteúdo prioritário
Contraste com branco: 12.6:1 (AAA)
```

```
Text/Gray
HEX: #7F8C8D
RGB: 127, 140, 141
Uso: Textos secundários, labels, hints, placeholders
Contraste com branco: 4.5:1 (AA)
```

```
Background/Light
HEX: #ECF0F1
RGB: 236, 240, 241
Uso: Fundos de tela, cards, separadores
```

```
White
HEX: #FFFFFF
RGB: 255, 255, 255
Uso: Fundos principais, texto em botões escuros
```

```
Border/Light
HEX: #BDC3C7
RGB: 189, 195, 199
Uso: Bordas de inputs, separadores, dividers
```

### Cores de Status

```
Success
HEX: #2ECC71
RGB: 46, 204, 113
Uso: Confirmações, metas atingidas
```

```
Warning
HEX: #F39C12
RGB: 243, 156, 18
Uso: Avisos, atenção necessária
```

---

## ✍️ Tipografia

### Fonte Principal
**Família:** Inter (Google Fonts)
**Fallback:** -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif

### Escala Tipográfica

#### Heading/XLarge
- **Tamanho:** 28px
- **Peso:** Bold (700)
- **Altura de linha:** 36px (1.29)
- **Cor:** #2C3E50
- **Uso:** Títulos de páginas, valores grandes (saldo)

#### Heading/Large
- **Tamanho:** 24px
- **Peso:** Bold (700)
- **Altura de linha:** 32px (1.33)
- **Cor:** #2C3E50
- **Uso:** Títulos de seções, headers

#### Heading/Medium
- **Tamanho:** 18px
- **Peso:** SemiBold (600)
- **Altura de linha:** 24px (1.33)
- **Cor:** #2C3E50
- **Uso:** Subtítulos, títulos de cards

#### Body/Large
- **Tamanho:** 16px
- **Peso:** Regular (400)
- **Altura de linha:** 24px (1.5)
- **Cor:** #2C3E50
- **Uso:** Textos principais, descrições

#### Body/Regular
- **Tamanho:** 14px
- **Peso:** Regular (400)
- **Altura de linha:** 20px (1.43)
- **Cor:** #2C3E50 ou #7F8C8D
- **Uso:** Textos secundários, listas

#### Caption/Small
- **Tamanho:** 12px
- **Peso:** Regular (400)
- **Altura de linha:** 16px (1.33)
- **Cor:** #7F8C8D
- **Uso:** Labels, hints, timestamps

#### Button/Text
- **Tamanho:** 16px
- **Peso:** SemiBold (600)
- **Altura de linha:** 20px (1.25)
- **Cor:** #FFFFFF (em botões) ou #27AE60 (em links)
- **Uso:** Textos de botões, CTAs

---

## 🔘 Componentes

### Botões

#### Primary Button (CTA Principal)
```
Dimensões: 358px × 48px (largura total - margens)
Altura: 48px (área de toque adequada)
Border Radius: 12px
Background: #27AE60
Text: 16px, SemiBold, #FFFFFF
Shadow: 0px 4px 8px rgba(39, 174, 96, 0.2)
Padding: 14px 24px

Estados:
- Hover: Background #229954
- Active: Background #1E8449
- Disabled: Background #BDC3C7, Text #7F8C8D
```

#### Secondary Button
```
Dimensões: 358px × 48px
Border: 2px solid #27AE60
Border Radius: 12px
Background: Transparent
Text: 16px, SemiBold, #27AE60
Padding: 12px 24px

Estados:
- Hover: Background rgba(39, 174, 96, 0.05)
- Active: Background rgba(39, 174, 96, 0.1)
```

#### Destructive Button
```
Dimensões: 358px × 48px
Border Radius: 12px
Background: #E74C3C
Text: 16px, SemiBold, #FFFFFF
Shadow: 0px 4px 8px rgba(231, 76, 60, 0.2)
```

#### Icon Button (Floating Action)
```
Dimensões: 56px × 56px
Border Radius: 28px (circular)
Background: #27AE60
Icon: 24px, #FFFFFF
Shadow: 0px 8px 16px rgba(39, 174, 96, 0.3)
Posição: Center bottom, 16px do fundo
```

### Cards

#### Card Padrão
```
Largura: 358px (auto-ajustável)
Padding: 16px
Border Radius: 16px
Background: #FFFFFF
Shadow: 0px 2px 8px rgba(0, 0, 0, 0.08)
Border: none

Espaçamento interno:
- Entre elementos: 12px
- Título e conteúdo: 8px
```

#### Card Destaque (Saldo)
```
Largura: 358px
Padding: 20px
Border Radius: 20px
Background: Linear gradient (135deg, #27AE60 0%, #229954 100%)
Shadow: 0px 8px 16px rgba(39, 174, 96, 0.25)
Text Color: #FFFFFF
```

### Inputs

#### Text Input Padrão
```
Largura: 358px (ou dentro do container)
Altura: 56px
Border Radius: 8px
Border: 1px solid #BDC3C7
Background: #FFFFFF
Padding: 16px

Label:
- Posição: Acima do input (8px de espaço)
- Tamanho: 14px, SemiBold, #2C3E50

Placeholder:
- 16px, Regular, #7F8C8D

Estados:
- Focus: Border 2px solid #27AE60
- Error: Border 2px solid #E74C3C
- Disabled: Background #ECF0F1, Border #BDC3C7
```

#### Select / Dropdown
```
Largura: 358px
Altura: 56px
Border Radius: 8px
Border: 1px solid #BDC3C7
Background: #FFFFFF
Padding: 16px
Icon: Chevron-down (16px) à direita
```

### Navegação Inferior (Bottom Navigation)

```
Dimensões: 390px × 72px
Background: #FFFFFF
Border Top: 1px solid #ECF0F1
Shadow: 0px -2px 8px rgba(0, 0, 0, 0.05)
Padding: 8px 0px

Items (4 itens):
- Largura por item: 97.5px (390 / 4)
- Altura: 56px
- Alinhamento: Center

Cada Item:
- Icon: 24px × 24px
- Label: 12px, Regular
- Espaçamento icon-label: 4px

Estados:
- Ativo: Icon e Text #27AE60
- Inativo: Icon e Text #7F8C8D
```

### Header

```
Altura: 64px (sem status bar) ou 108px (com status bar)
Background: #FFFFFF ou Transparente (sobre gradiente)
Padding: 16px horizontal
Shadow: 0px 2px 4px rgba(0, 0, 0, 0.05) (quando com fundo)

Elementos:
- Título: 18px, SemiBold, #2C3E50, centralizado
- Botão voltar: Icon 24px, esquerda (16px margem)
- Ações: Icon 24px, direita (16px margem)
```

### Ícones

```
Biblioteca: Feather Icons
Tamanhos:
- Navegação e headers: 24px
- Botões e inline: 20px
- Status e badges: 16px

Cores:
- Ativos: #27AE60
- Inativos: #7F8C8D
- Destaque: #3498DB
- Alerta: #E74C3C
```

---

## 📊 Gráficos

### Gráfico de Pizza (Dashboard)
```
Dimensões: 200px × 200px
Espessura: 30px (donut chart)
Centro: Valor total ou percentual

Cores por categoria:
- Alimentação: #E74C3C (vermelho)
- Transporte: #F39C12 (laranja)
- Moradia: #3498DB (azul)
- Lazer: #9B59B6 (roxo)
- Saúde: #1ABC9C (turquesa)
- Educação: #34495E (cinza escuro)
- Outros: #95A5A6 (cinza claro)
```

### Gráfico de Barras (Relatórios)
```
Largura: 358px
Altura: 200px
Barras:
- Largura: Auto (depende do número de meses)
- Espaçamento: 8px
- Border Radius: 4px (topo)

Cores:
- Receitas: #27AE60
- Despesas: #E74C3C

Eixos:
- Linhas: 1px, #ECF0F1
- Labels: 12px, Regular, #7F8C8D
```

### Barra de Progresso (Metas)
```
Largura: 100% do container
Altura: 8px
Border Radius: 4px
Background: #ECF0F1

Progresso:
- Background: #27AE60
- Border Radius: 4px
- Animation: smooth transition 0.3s
```

---

## 📱 Estrutura das Telas

### 1. Tela de Onboarding
```
Layout:
- Logo/Ícone: Centro, 120px × 120px, margem superior 120px
- Título: 24px, Bold, 24px abaixo do ícone
- Subtítulo: 16px, Regular, #7F8C8D, 12px abaixo
- Botão: 48px altura, 32px do fundo da tela
- Skip/Próximo: 16px, SemiBold, #3498DB, canto superior direito

Cores:
- Background: #FFFFFF ou gradiente suave
```

### 2. Tela de Login
```
Layout:
- Logo: Topo centro, margem superior 80px
- Título: "Entrar", 24px Bold, 40px abaixo do logo
- Inputs: 2 campos (Email + Senha), 16px entre eles
- Botão: "Entrar", 24px abaixo dos inputs
- Link: "Esqueci a senha", 16px abaixo do botão
- Divider: "ou", 24px abaixo
- Link: "Criar conta", 16px abaixo

Background: #FFFFFF
```

### 3. Tela de Dashboard (Principal)
```
Layout:
- Header: 64px altura
  - Saudação: "Olá, Marina" (16px, SemiBold)
  - Notificações: Icon 24px, direita
  
- Card Saldo: 120px altura, 16px margem top
  - Label: "Saldo disponível" (12px, #FFFFFF 80%)
  - Valor: "R$ 2.450,00" (28px, Bold, #FFFFFF)
  
- Resumo Mensal: 2 colunas, 16px margem top
  - Receitas (verde) | Despesas (vermelho)
  - Valor + Label (14px)
  
- Gráfico Pizza: 200px × 200px, 24px margem top
  - Título: "Gastos por categoria" (18px, SemiBold)
  
- Lista Transações: 24px margem top
  - Título: "Transações recentes" (18px, SemiBold)
  - Itens: 64px altura cada
  
- Bottom Navigation: 72px altura, fixo no fundo

Scroll: Vertical, começa após header
```

### 4. Modal de Nova Transação
```
Layout:
- Overlay: Background rgba(0, 0, 0, 0.5)
- Container: 358px largura, auto altura
- Posição: Centro da tela
- Border Radius: 20px (topo)
- Background: #FFFFFF
- Padding: 24px

Conteúdo:
- Handle: 40px × 4px, #BDC3C7, centro topo
- Título: "Nova transação" (20px, Bold)
- Tipo: Segmented control (Despesa/Receita), 16px abaixo
- Input Valor: 56px altura, 16px abaixo
- Select Categoria: 56px altura, 16px abaixo
- Input Descrição: 56px altura, 16px abaixo, opcional
- Botão Salvar: 48px altura, 24px abaixo
```

### 5. Tela de Relatórios
```
Layout:
- Header: "Relatórios" (18px, SemiBold, centro)
- Filtro Período: Tabs horizontais, 16px margem top
  - "Este mês" | "3 meses" | "6 meses" | "Ano"
- Resumo Cards: 2 colunas, 16px margem top
  - Total Receitas | Total Despesas
- Gráfico Barras: 200px altura, 24px margem top
- Cards Categorias: Lista, 16px margem top
  - Nome, ícone, valor, % do total

Background: #ECF0F1
Cards: #FFFFFF
```

### 6. Tela de Metas
```
Layout:
- Header: "Minhas Metas" (18px, SemiBold, centro)
- Card Meta (repetível):
  - Ícone: 48px × 48px, círculo colorido
  - Título: 18px, SemiBold
  - Progresso: Barra 8px altura
  - Valores: "R$ X de R$ Y" (14px)
  - Percentual: "60%" (16px, Bold, #27AE60)
  - Prazo: "Faltam 4 meses" (12px, #7F8C8D)
  - Padding: 16px
  - Margin bottom: 16px
- Botão Add: Floating, 56px × 56px, bottom right

Background: #ECF0F1
Cards: #FFFFFF
```

---

## 🔄 Interações e Animações

### Transições entre Telas
```
Tipo: Slide horizontal
Duração: 300ms
Easing: ease-in-out
```

### Botões
```
Hover: Scale 1.02, duração 150ms
Active: Scale 0.98, duração 100ms
Ripple: Ondas concêntricas, 400ms
```

### Modal/Bottom Sheet
```
Entrada: Slide up from bottom, 400ms, ease-out
Saída: Slide down, 300ms, ease-in
Overlay: Fade in 200ms / Fade out 150ms
```

### Cards
```
Hover: Shadow aumenta (y: 4px), 200ms
Loading: Skeleton shimmer, 1.5s loop
```

---

## ♿ Acessibilidade

### Contraste (WCAG 2.1 AA)
- Textos normais (≤18px): Mínimo 4.5:1
- Textos grandes (>18px): Mínimo 3:1
- Elementos UI: Mínimo 3:1

### Área de Toque
- Mínimo: 44px × 44px (iOS) / 48px × 48px (Android)
- Espaçamento entre elementos tocáveis: 8px

### Semântica
- Labels descritivos em todos os inputs
- Alt text em ícones informativos
- ARIA labels quando necessário
- Ordem de foco lógica

### Modo Escuro (Opcional)
```
Background: #1E1E1E
Cards: #2C2C2C
Text: #FFFFFF
Text Secondary: #B0B0B0
```

---

## 📏 Status Bar & Safe Areas

### iOS Status Bar
```
Altura: 44px (iPhone 14 Pro)
Cor: Dynamic (branca ou preta conforme fundo)
```

### Safe Area
```
Top: 44px (status bar)
Bottom: 34px (home indicator)
Sides: 0px
```

### Considerações
- Conteúdo importante deve estar fora das safe areas
- Bottom navigation altura total: 72px + 34px safe area = 106px

---

## 📦 Assets e Recursos

### Ícones Necessários
```
Navegação:
- home (dashboard)
- bar-chart-2 (relatórios)
- target (metas)
- user (perfil)

Ações:
- plus (adicionar)
- edit-2 (editar)
- trash-2 (deletar)
- check (confirmar)
- x (fechar)

Categorias:
- shopping-bag (compras)
- coffee (alimentação)
- car (transporte)
- home (moradia)
- heart (saúde)
- book (educação)
- smile (lazer)
```

### Ilustrações
- Onboarding: Financeiro (verde/azul)
- Empty states: Minimalistas, 200px × 200px
- Celebração: Meta atingida (confete/troféu)

---

## 🎯 Fluxo de Navegação

```
Onboarding → Login → Dashboard
                        ↓
            ┌───