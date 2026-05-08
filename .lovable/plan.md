
# Landing Page — Matheus Barbosa | Perícia Forense de Imagens de IA

Landing page única, rápida e objetiva, focada em converter o visitante em uma conversa no seu WhatsApp. Visual sóbrio (Navy Trust + Urbanist/Epilogue) transmitindo autoridade técnica e jurídica.

## Estrutura da página (de cima para baixo)

1. **Header fixo minimalista**
   - "Matheus Barbosa" à esquerda, com a linha fina "OAB/PR 132397 · Habilitado CAJU-TJPR".
   - Botão "Falar no WhatsApp" à direita.

2. **Hero**
   - Título: "Perícia Forense de Imagens Geradas ou Manipuladas por IA".
   - Subtítulo posicionando para quem é: processos judiciais, bancos, financeiras, proteção veicular e campanhas políticas.
   - Selo de credenciais em destaque: **Matheus Barbosa — OAB/PR 132397 · Perito habilitado no CAJU-TJPR**.
   - Dois CTAs: "Solicitar análise no WhatsApp" e "Pedir orçamento".

3. **Para quem atendo** (5 cards)
   - Advogados e processos judiciais
   - Bancos e financeiras (fraudes em selfies, documentos, comprovantes)
   - Associações de proteção veicular (sinistros com imagens suspeitas)
   - **Partidos políticos e candidatos** (deepfakes, montagens e manipulações em campanhas)
   - Empresas e seguradoras em geral

4. **O que é entregue**
   - Análise técnica de autenticidade da imagem
   - Detecção de geração por IA / deepfake / manipulação
   - Laudo pericial com validade para uso processual
   - Pareceres técnicos e assistência técnica em processos

5. **Sobre / Credenciais** (com sua foto)
   - Foto sua à esquerda, texto à direita.
   - Apresentação como **Matheus Barbosa, OAB/PR 132397**, perito habilitado no **CAJU-TJPR**.
   - Reforço da metodologia técnica, ferramentas forenses, sigilo e cadeia de custódia.

6. **Como funciona** (3 passos)
   - 1. Você envia o caso pelo WhatsApp/formulário · 2. Avaliação preliminar e orçamento · 3. Emissão do laudo no prazo combinado.

7. **FAQ curto** (4–6 perguntas)
   - Ex.: "O laudo tem validade em juízo?", "Atende casos eleitorais com urgência?", "Quais formatos de imagem aceita?", "Prazo médio?", "Atende fora do PR?".

8. **CTA final + Contato**
   - Formulário simples (nome, e-mail, telefone, tipo de demanda — incluindo "Partido/Campanha política" — e descrição do caso) que, ao enviar, abre o WhatsApp com a mensagem já preenchida.
   - Botão direto de WhatsApp e e-mail como alternativa.

9. **Botão flutuante de WhatsApp** visível em toda a página.

10. **Footer** enxuto: Matheus Barbosa · OAB/PR 132397 · Habilitado CAJU-TJPR · contato · ano.

## Captação de leads

- **Formulário** com validação Zod (nome, e-mail, telefone, tipo de cliente, descrição do caso).
- **Ação ao enviar**: monta mensagem formatada e abre `https://wa.me/<seu-numero>?text=...` em nova aba — sem backend.
- **Botão flutuante de WhatsApp** sempre visível (mobile e desktop).

## Identidade visual

- **Paleta Navy Trust**: fundo claro `#e8edf3` / branco, primário `#0f1b3d`, acentos `#1e3a5f` e `#3b6fa0`.
- **Tipografia**: Urbanist (títulos) + Epilogue (corpo), via Google Fonts.
- **Tom visual**: sóbrio, espaçoso, ícones outline, sutis detalhes técnicos no hero. Mobile-first.

## Detalhes técnicos

- Página única em `src/routes/index.tsx` com seções em `src/components/landing/`.
- Sem backend / sem Lovable Cloud — formulário envia direto via `wa.me`.
- `react-hook-form` + `zod` para validação.
- SEO em `head()`: title, description e og tags com palavras-chave "perícia forense de imagens IA, deepfake, laudo pericial, CAJU TJPR, OAB PR".
- Tokens de cor Navy Trust em `oklch` no `src/styles.css` (light mode).

## O que vou precisar depois

- Número de WhatsApp (com DDI/DDD) para o link `wa.me`.
- E-mail de contato profissional.
- Sua foto (você já avisou que vai enviar) — uso um placeholder até chegar.
