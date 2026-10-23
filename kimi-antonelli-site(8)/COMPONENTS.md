# Componentes Modulares: Kimi Antonelli (#12)
> **Identidade Visual**: Mercedes-AMG Petronas F1 Team / Lunar Works Palette  
> **Piloto**: Andrea Kimi Antonelli (Monolugar #12)  
> **Design System**: Adaptado a partir da extração `/extract-ds` com fluid scaling, curvas esportivas e cinética F1.

---

## 1. Paleta de Cores Oficial Mercedes-AMG Petronas F1

| Nome do Token | Valor Hex | Função na Interface |
|---|---|---|
| **Deep Teal** | `#004146` | Fundo escuro principal do site, overlay do menu tela-cheia e seções. |
| **Rich Teal** | `#018076` | Tom secundário, superfícies de cartões e molduras de bordas. |
| **Petronas Cyan** | `#03BFB5` | Cor de destaque primária: botões CTA, badges, anéis de foco, sublinhados dinâmicos e telemetria. |
| **Silver Gray** | `#949398` | Cinzento prateado para metadados, subtítulos, datas e textos de suporte. |
| **Off-White** | `#EFF5F9` | Branco suave para títulos de alto impacto, textos corridos e legibilidade pura sem fadiga ocular. |

---

## 2. Estrutura Modular de Arquivos

```
D:\Downloads\kimi-antonelli\
├── index.html                  # Preview completo funcional e responsivo em Português
├── COMPONENTS.md               # Guia técnico e documentação modular
├── styles\
│   ├── fonts.css               # Fontes Brier e Mona Sans Variable (WOFF2 embutidas)
│   ├── variables.css           # Tokens oficiais Mercedes-AMG Petronas F1 (:root)
│   └── components.css          # Estilização de todos os componentes e responsividade
├── scripts\
│   └── main.js                 # Engine de SplitText, menu elíptico e rolagem suave
└── components\
    ├── navbar.html             # Componente 1: Header / Navbar com Logo e Menu
    ├── hero.html               # Componente 2: Hero Section com foto real e telemetria
    ├── trajectory.html         # Componente 3: Trajetória & Conquistas (Bio Histórica)
    ├── news-card.html          # Componente 4: Grid e Card de Notícias F1
    ├── product-card.html       # Componente 5: Vitrine da Loja Oficial (Merch)
    ├── calendar.html           # Componente 6: Calendário Oficial de Corridas F1
    └── partners-banner.html    # Componente 7: Banner e Marquee de Patrocinadores
```

---

## 3. Resumo dos Componentes Implementados

### 1. Navbar / Header (`components/navbar.html`)
- **Logo**: Tipografia display `KIMI ANTONELLI` com badge `#12` em Petronas Cyan.
- **Pílula de Navegação Translúcida**: Vidro fosco com efeito `backdrop-filter: blur(16px)` em Deep Teal com borda Rich Teal.
- **Links**: `INÍCIO`, `TRAJETÓRIA`, `NOTÍCIAS`, `LOJA OFICIAL`, `PARCEIROS`.
- **Botão Loja**: CTA voltado ao e-commerce com ícone SVG de sacola e animação *SplitText*.
- **Menu Tela-Cheia**: Abertura por *clip-path* elíptico suave em `0.75s cubic-bezier(0.65, 0.05, 0, 1)`.

### 2. Hero Section (`components/hero.html`)
- **Badge**: Indicador com ponto pulsante turquesa: `MERCEDES-AMG PETRONAS F1 TEAM • #12`.
- **Tipografia Gigante**: `KIMI ANTONELLI` em escala de impacto heroico (8.25rem na fonte Brier, com destaque em `#03BFB5`).
- **Subtítulo**: *"Official Site of Kimi Antonelli. Rising Star. Mercedes-AMG F1 Junior Driver."*
- **Ações**: Botão primário `DISCOVER THE STORY` com micro-interação de texto e botão secundário `ÚLTIMAS NOTÍCIAS`.
- **Foto Real de Capa**: Fotografia de Kimi Antonelli no paddock com uniforme oficial Mercedes-AMG F1, moldura aerodinâmica e painel de telemetria flutuante (Monolugar #12, Equipe Mercedes, Status F1 Driver).

### 3. Trajetória & Conquistas (Bio Histórica) (`components/trajectory.html`)
Seção dedicada aos 4 pilares históricos da carreira de Kimi:
1. **Origem e Karting (2014–2021)**: Nascido em Bolonha, Itália (filho de Marco Antonelli). Bicampeão Europeu CIK-FIA (2020 e 2021), campeão do WSK Euro Series e ingresso na Mercedes Junior Team.
2. **Domínio na Fórmula 4 (2022)**: Campeão do Campeonato Italiano de Fórmula 4 e do ADAC F4 Alemão pela Prema Racing, além da medalha de ouro na Copa F4 do FIA Motorsport Games.
3. **Campeão Regional (2023)**: Campeão da Fórmula Regional Europeia (FRECA) e da Fórmula Regional do Oriente Médio (FRMEC).
4. **Fórmula 2 e Chegada à Fórmula 1 (2024–2025)**: Promovido diretamente da FRECA para a Fórmula 2 com vitórias em Silverstone e Budapeste, anunciado como piloto titular da Mercedes-AMG Petronas F1 Team no carro #12.

### 4. Grid de Notícias (`components/news-card.html`)
- Grid de 3 colunas responsivo.
- Imagens reais do monolugar Mercedes-AMG F1 W15 na pista, engenharia de telemetria em Brackley e capacete oficial com as cores da Itália e da Mercedes.
- Efeito hover zoom suave (`scale(1.06)`) e traço de realce turquesa animado (`.high-line-reveal`).

### 5. Vitrine da Loja Oficial (`components/product-card.html`)
- Cards com produtos e colecionáveis oficiais de Kimi Antonelli:
  1. **Hot Wheels Mercedes-AMG F1 Kimi Antonelli (Mattel)**: miniatura em metal premium com acabamento fiel, badge `OFERTA -29%`, avaliações ★ 4.8 e preço de R$ 70,95.
  2. **Funko Pop! Racing Kimi Antonelli #13**: boneco colecionável de vinil licenciado oficial, badge `FUNKO POP! RACING`, avaliações ★ 4.7 e preço de R$ 854,05.
  3. **Quadro Kimi Antonelli F1 com Moldura e Vidro**: poster fotográfico de alta definição com vidro e moldura preta, badge `OFERTA IMPERDÍVEL`, avaliações ★ 5.0 e preço de R$ 49,48.
- Badges de destaque, avaliações, condições de parcelamento e botões de compra com o texto `SHOP NOW` e animação SplitText.

### 6. Calendário Oficial de Corridas F1 (`components/calendar.html`)
- **Spotlight (Próxima Etapa)**: Destaque com telemetria (distância, voltas, recorde, cronograma do fim de semana em horário de Brasília).
- **Filtros Interativos**: `TODAS AS ETAPAS (24)`, `EUROPA`, `AMÉRICAS`, `ÁSIA & ORIENTE MÉDIO`, `RODADAS SPRINT ⚡` e `CORRIDAS EM CASA 🇮🇹`.
- **Grid Completo de 24 Grandes Prêmios**: Rondas com bandeira do país, circuito, datas, voltas, quilometragem e badges especiais (`HOME RACE KIMI 🇮🇹`, `CASA MERCEDES-AMG 🇬🇧`, `SPRINT ⚡`).

### 7. Banner de Patrocinadores (`components/partners-banner.html`)
- Trilho de *marquee* infinito com velocidade constante de 28s e máscara lateral de gradiente linear suave (`mask-image: linear-gradient(90deg, transparent, white 8%, white 92%, transparent)`).
- Logotipos: **Petronas** (em `#03BFB5`), **Mercedes-AMG**, **Puma**, **Tommy Hilfiger**, **IWC Schaffhausen**, **TeamViewer**, **Pirelli** e **Monster Energy**.

---

## 4. Como Executar

Basta dar duplo clique ou abrir o arquivo `D:\Downloads\kimi-antonelli\index.html` em qualquer navegador moderno. Todo o CSS, fontes e lógica estão integrados localmente de forma autônoma.


---

## 5. Identidade visual de alta performance — F1 / e-sports

O `index.html` aplica uma interpretação original de estética F1/e-sports, preservando estrutura e conteúdo do site de Kimi e seguindo as diretrizes visuais mais recentes:

- **Paleta**: preto `#000000`, grafite `#121212`, branco `#FFFFFF`, cinza `#A0A0A0` e neon `#CCFF00`.
- **Tipografia**: Inter e Space Grotesk como sans-serif geométricas; títulos em caixa alta, pesos altos e tracking compacto.
- **Superfícies**: cards grafite com bordas sutis, brilho lima no hover, traços diagonais e grade técnica discreta.
- **Ações**: CTAs preenchidos em neon, botões secundários vazados, animações rápidas e foco visível.
- **Seções**: hero, notícias, produtos, calendário, galeria, patrocinadores e rodapé usam a paleta escura; o banner existente foi escurecido por CSS.
- **Responsividade**: grids e navegação adaptam-se a telas menores, com suporte à preferência de movimento reduzido.

As imagens principais estão embutidas como WebP data URIs no HTML; o ZIP também inclui os assets originais e esta documentação.


### Galeria conceitual Kimi / Engenharia e retratos
- Seção `#concept-gallery` incluída logo após o hero, com acesso pelo menu principal e pelo menu expandido.
- Composição assimétrica responsiva: retrato cutaway vertical e galeria de cinco cartões em leque horizontal.
- Imagens convertidas para WebP e embutidas como data URI para manter o `index.html` autônomo sem requests extras; carregamento lazy e decoding assíncrono na seção.
- Legendas e textos alternativos descrevem as imagens para acessibilidade; em telas estreitas, os dois cards empilham numa coluna.


### Ajuste de apresentação da vitrine de produtos
- Cards em grafite claro `#1E1E1E` e área de mídia em `#252525`, com radial glow suave no fundo.
- Removidos tratamentos escuros das imagens e aplicado aumento moderado de brilho/contraste.
- Hover com zoom leve, borda neon fina e brilho externo controlado.


### Carrossel de patrocinadores
- Marquee contínuo em velocidade reduzida para um ciclo de 100 segundos; as cópias existentes mantêm o loop sem emendas.
- Animação pausa ao passar o mouse ou ao focar a área por teclado.
- Logos em cinza monocromático com realce neon e brilho discreto no hover.
- Com `prefers-reduced-motion`, a animação é desativada e a faixa permanece acessível por rolagem horizontal.


## 6. Experiência de loja e conversão

- **Contador**: cronômetro visual no hero para 1º de novembro de 2026 às 20h (horário de Brasília), marcado explicitamente como demonstrativo; atualizar para a data real antes de campanha.
- **Badges e filtros**: tags de destaque sem alegações de estoque; filtros de miniaturas, pôsteres, vestuário e colecionáveis.
- **Carrinho lateral**: sacola com quantidades, remoção de itens, subtotal em tempo real e persistência local no navegador. Checkout é apenas um aviso: gateway, cálculo de frete e processamento de pedidos não estão conectados.
- **Wishlist**: favoritos por produto persistidos localmente.
- **Pit Stop Reviews**: formulário de comentário, nota e foto opcional; avaliações são locais e não verificadas. Nenhum depoimento ou imagem de comprador foi criado artificialmente. Para avaliações públicas reais, é necessário integrar backend/moderação e obter conteúdo consentido.
- **Pit Stop Club**: formulário local demonstrativo de captura; e-mails não são enviados a uma plataforma de newsletter até conectar um serviço. Os benefícios (10%, frete grátis, acesso antecipado) são conteúdo promocional solicitado e devem corresponder à oferta real na publicação.
- **Pagamento e segurança**: identificadores PIX/cartão e selo de segurança são apenas indicativos visuais; não há gateway ou certificação conectados.
- **Contraste**: tratamentos claros de imagem e fundos grafite dos produtos são preservados.


## 7. Proteção de colecionáveis e alertas VIP

- **Embalagem especial**: barra de confiança na loja e selo em cada card informando “Embalagem Protegida Anti-Amassado”; a faixa geral mantém o aviso detalhado sobre tubo rígido/caixa protetora. A afirmação deve corresponder ao processo real antes do site ser usado em vendas. A afirmação deve corresponder ao processo real de expedição antes do site ser usado em vendas.
- **Aviso VIP de drops**: faixa dedicada e atalho flutuante para cadastro de e-mail ou WhatsApp, com validação básica do contato. No protótipo, os dados ficam somente em `localStorage`; não existe grupo de WhatsApp ou plataforma de mensagens conectada e nenhum alerta é enviado.
- **Privacidade/produção**: conectar backend com consentimento, aviso de privacidade e integração ao canal oficial antes de coletar contatos em produção.

## 8. Catálogo restaurado pelo usuário (8 cards)

A loja apresenta oito produtos e o filtro “TODOS 08”. Os três cards recuperados do backup anterior são: camiseta oversized KA12 (R$ 189,90; ★ 4.8, 64 avaliações), pôster Fine Art The Next Gen (R$ 59,90; ★ 4.9, 45 avaliações) e chaveiro metálico KA12 (R$ 39,90; ★ 4.7, 112 avaliações). Os preços e dados são os do protótipo anterior e devem ser confirmados antes da publicação comercial.

Os outros cinco cards mantêm os dados já definidos: Hot Wheels R$ 70,95 (de R$ 99,90); Funko Pop! R$ 854,05; quadro R$ 49,48 (de R$ 53,70); boné R$ 249,90; capacete 1:5 R$ 389,00. Títulos, avaliações, descrições, badges, favoritos e ações de sacola continuam no array JavaScript.

## 9. Fidelidade, vestuário, mural de fãs e FAQ

- **Pit Stop Points**: painel de mecânica de pontos demonstrativa (1 por R$ 1; 100 pela inscrição; 50 por compartilhamento; 500 por cupom de R$ 15), simulador local e compartilhamento manual. Nenhum ponto é creditado; validar regulamento e conectar backend antes de anunciar como programa ativo.
- **Guia de tamanhos**: link no card do boné abre diálogo acessível com medida de referência (56–60 cm ajustável). A medida é ilustrativa e deve ser conferida com fabricante.
- **Na Pista com os Fãs**: mural inicialmente vazio. Pode pré-visualizar até oito fotos/vídeos consentidos, até 20 MB por arquivo, usando URLs de objeto desta sessão; arquivos não são salvos, enviados ou publicados.
- **FAQ**: respostas transparentes sobre autenticidade/licenciamento, embalagem, frete e trocas. Não há documentação de autenticidade, confirmação de operação logística, prazo ou política de devolução integrada; configurar antes de vender.
- **Catálogo**: contador “TODOS 08”; oito cards gerados pelo array JavaScript. Distribuição atual: miniaturas 0, pôsteres 2, vestuário 2, colecionáveis 4. Todas as imagens usam assets WebP locais e fallbacks embutidos no HTML.
- **Cards**: todos mostram selo “Embalagem Protegida Anti-Amassado”; o link de vestuário está nomeado “Guia de Tamanhos”. A sacola lateral abre sem recarregar, com subtotal e persistência local.

## 10. Controles da sacola corrigidos

- A renderização gera cada linha como `.cart-item` com os elementos `.cart-item-info`, `.cart-item-title`, `.cart-item-price`, `.cart-item-actions`, `.btn-qty-minus`, `.cart-item-qty`, `.btn-qty-plus` e `.btn-remove-item`. Cada botão recebe seu listener ao ser criado.
- `window.changeQuantity(id, delta)` e `window.removeFromCart(id)` ficam acessíveis globalmente e normalizam IDs numéricos ou chaves `ka12-N` para o formato do catálogo.
- Aumentar/diminuir atualiza quantidade, contador e subtotal; quantidade zero remove o item. `×` remove a linha imediatamente.
- Ao esvaziar a sacola, o drawer mostra “Sua sacola está vazia” e o botão “Continuar Comprando”, que fecha o drawer e retorna à loja. O checkout fica desabilitado sem itens.

## 11. Imagens do catálogo (8 cards)

Todas as imagens foram substituídas por arquivos locais WebP em `assets/`, com fallback base64 correspondente no HTML, para que os cards permaneçam visíveis sem dependência de hotlink remoto. A geração das miniaturas preservou o aspecto original; imagens grandes foram reduzidas para no máximo 1600 px de lado para acelerar o carregamento.

Mapeamento: Hot Wheels Mercedes/Kimi (`product-hot-wheels-kimi-antonelli.webp`); Funko Pop! #13 (`product-funko-kimi-antonelli-13.webp`); quadro emoldurado de corrida (`product-quadro-kimi-antonelli.webp`); boné Mercedes preto (`product-bone-mercedes-kimi-12.webp`); capacete 1:5 (`product-capacete-kimi-antonelli-15.webp`); camiseta KA12 (`product-camiseta-ka12-speed-dynamics.webp`); pôster Kimi Antonelli (`product-poster-kimi-antonelli-fine-art.webp`); chaveiro metálico de volante F1 (`product-chaveiro-volante-formula-1.webp`).

As fotos foram selecionadas em páginas de produtos de varejistas e lojas oficiais. A licença comercial não foi confirmada para os arquivos; disponibilidade pública não concede direito de reprodução. Obter autorização dos respectivos titulares/licenciantes antes de usar em uma loja pública. A imagem da camiseta corresponde a uma camiseta KA12, mas a fonte não confirma corte oversized; a do chaveiro mostra um volante metálico, uma das formas solicitadas, não o modelo exato de capacete KA12.
