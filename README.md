# Real Estate Camera Raw Skill

Skill para Codex que analisa imagens imobiliárias, renders de archviz, frames gerados por IA e fotos reais para sugerir valores exatos do **Filtro do Camera Raw no Adobe Photoshop 2026**.

O foco é um visual **imobiliário cinematográfico e realista**: fotografia profissional, cores controladas, vegetação natural, materiais limpos e sem saturação estourada típica de imagem gerada por IA.

## O que a skill faz

- Analisa interiores, fachadas, áreas externas, vistas aéreas, cenas com piscina, chuva, golden hour, blue hour e imagens noturnas.
- Sugere valores exatos para os painéis Luz, Cor, Efeitos, Curva Paramétrica e Misturador de Cores - HSL.
- Ajuda a manter consistência de cor entre várias imagens do mesmo projeto para workflows de vídeo imobiliário.
- Controla sinais comuns de IA, como verdes neon, céu saturado, materiais plásticos, excesso de laranja e contraste artificial.
- Recomenda máscaras locais quando o ajuste global não resolve céu, janela, vegetação, água, pele, fachada ou reflexos.

## Como instalar no Codex

No Codex, peça:

```text
Instale a skill do GitHub felipealmeidasid/Real-state-Filtro-Camera-Raw no caminho .
```

Depois de instalada, use:

```text
Use $real-estate-camera-raw para analisar estas imagens e sugerir valores exatos no Camera Raw com visual imobiliário cinematográfico e realista.
```

## Estrutura

```text
SKILL.md
references/
  camera-raw-real-estate-guide.md
agents/
  openai.yaml
```

## Observação importante

A skill foi calibrada para ser conservadora por padrão. `Realces` negativos fortes são usados quando há céu, sol, LEDs, janelas, lâmpadas ou reflexos realmente problemáticos. `Textura` alta é reservada para aéreas, maquetes, obras, pedra, telhado, asfalto e materiais com detalhe; em pele, água, chuva, vidro, céu e paredes lisas ela deve ficar baixa.
