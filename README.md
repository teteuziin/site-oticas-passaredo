# Site — Óticas Passaredo (@passaredo_) — FASE 2, empresa nº2

Pacote em estrutura de pastas (`index.html` + `media/`), pronto para o GitHub **somente após aprovação do usuário**. Nada foi publicado.

## Conceito — "A Bandeja"
O site se organiza como a bandeja rosa de apresentação dela: painéis bege/bordô com moldura dupla, filete dourado e o coração da marca no fecho superior. Sistema limpo estilo SaaS: uma mensagem por seção, paleta contida (bege + bordô, rosa como apoio), 2 tipografias (Fraunces + Jost), no máximo 1 destaque por seção.

## Seções
1. **Hero** — slogan + frase real dela como H1; vídeo real da loja Essência (vista mar) em autoplay mudo, numa moldura em arco; faixa do Novembro OFF.
2. **Novembro OFF** — R$ 123 (Sublime), R$ 123 (solares), 30% OFF demais linhas, no óculos completo; vídeo oficial da campanha com som.
3. **Coleções & Preços Fixos** — filtros (Todas / Preço fixo / Grifes e lentes), 4 cards com lightbox (Sublime R$ 249,90 · Clip-on 2-em-1 R$ 299,90 · Solares Clássica R$ 199,90 · Grifes e lentes Hoya/Zeiss/Essilor/Varilux) + **simulador** da condição do mês.
4. **Essência** — galeria das 8 fotos reais do tour da loja da Pituba, com lightbox.
5. **Vídeos** — trilho horizontal com 5 vídeos reais com som (pausa automática ao sair da tela, sem retomada).
6. **Serviços** — abas: Passa in Casa (taxa de R$ 50 devolvida; CTA direct do Instagram), Image Glasses By Lu, PassaMóvel, PassaMoney (R$ 1 = 1), Hora marcada.
7. **Lojas** — seletor com as 3 lojas ativas (Pituba/Essência, Iguatemi — nota 4,6 —, Lauro/Vilas), endereço, horário, telefone e rota no Google Maps.
8. **Rodapé** — logo oficial recortado da arte da marca, navegação e @passaredo_.

## Escolhas sinalizadas
- **Telefone (71) 99300-0188**: publicado no Google Places de todas as unidades, mas **não rotulado oficialmente como WhatsApp** em nenhum canal público. Usado como **telefone das lojas** (botão "Ligar para a loja"); o CTA de agendamento do Passa in Casa aponta para o **direct do Instagram**. Nenhum outro número foi inventado.
- **Não citadas**: Feira de Santana (atividade não confirmada) e as unidades fechadas (Ondina, Salvador Shopping Business).
- Frases do site são verbatim dela ou ancoradas em fatos verificados da ficha (`../oticas-passaredo-portfolio/README.md`). Zero texto genérico/de tutorial.

## Mídia
Tudo real, vindo de `../oticas-passaredo-portfolio/` (vídeos H.264+AAC com áudio confirmado por ffprobe; nunca embutir vídeo em base64). `media/marca/logo-passaredo.png` é recorte do logo branco sobre bordô da arte oficial dela. `media/posters/` são frames extraídos dos próprios vídeos.

## Checagens executadas (17/11/2026)
- Estrutura HTML validada (tags balanceadas); 20 referências de mídia, nenhuma faltando.
- Contraste WCAG AA calculado para todos os pares texto×fundo (mínimo 5,60:1 após ajuste do dourado).
- Testes de interação em DOM (jsdom): intro, menu mobile, filtros, simulador (R$ 123 / R$ 209,93 / —), abas de serviços e lojas, lightbox com navegação e Esc — todos passando.
- Auditoria de layout em render real (390/768/1440) não executável neste ambiente (o único Chromium da VM é bloqueado por política para uso headless); o layout foi construído em sistema rígido de 8px com breakpoints de empilhamento e segue para a conferência visual do usuário na prévia.
