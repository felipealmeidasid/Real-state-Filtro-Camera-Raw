---
name: real-estate-camera-raw
description: Analyze any user-provided image that needs professional Adobe Camera Raw Filter settings, especially AI-generated architectural visualization images, real estate photos, property marketing stills, and video storyboard frames, then prescribe exact Photoshop 2026 settings in Brazilian Portuguese for a cinematic, realistic, professional real estate look. Use when the user uploads interior, exterior, aerial, amenity, facade, pool, golden hour, blue hour, night, render, Seedance/Kling/Midjourney/DALL-E/GPT Image, real photo, or mixed project images and asks for "avalia essa imagem", "configura o Camera Raw", "filtro de camera raw", "settings para essa imagem", "grading archviz", "correção de cor", "deixar mais realista", "mais limpa/profissional", "cinematográfico realista", or batch consistency for real estate video workflows.
---

# Real Estate Camera Raw

## Core Workflow

1. Classify the image before prescribing values: exterior diurno, exterior golden hour/sunset, exterior noturno/blue hour, interior luz natural, interior luz artificial, aerial/drone, piscina/água, close-up material/produto, or mixed batch.
2. Evaluate the image through three professional lenses, without exposing long reasoning:
   - Architectural photographer: lighting condition, dynamic range, exposure, composition stress points, highlight clipping, crushed shadows, and white balance.
   - Colorist: dominant palette, color cast, oversaturation, sky/water/vegetation fidelity, skin if people are present, and AI color contamination.
   - Retoucher: sharpness, AI softness, smearing, repeated texture, plastic materials, haze, noise, banding, and material realism.
3. Use cinematic realistic real estate grading as the default style: professional photographic depth, controlled contrast, believable warmth, clean materials, and no blown-out AI saturation.
4. Prescribe exact Camera Raw Filter values, not ranges. Use the reference ranges only to choose a single final number.
5. Keep values conservative by default. Most sliders should stay between -30 and +30 unless the image clearly needs stronger correction.
6. Treat Realces and Textura as contextual controls, not automatic heavy moves. Strong negative Realces are justified for sun, sky, LEDs, windows, wet reflections, and lamps; high Textura is justified for aerials, maquettes, construction sites, stone, roof tiles, asphalt, and detailed materials.
7. Prefer realistic architectural photography over stylized grading. Protect believable whites, wood, stone, concrete, glass, metal, vegetation, sky, water, and human skin.
8. Separate global adjustments from local needs. If a bright sky and dark interior need opposite treatment, give the primary global settings and mention masks/local adjustments.
9. For batches, define the shared base grade plus exceptions so consecutive video shots do not jump in warmth, brightness, sky color, greenery, water color, wall neutrality, or black point.

Always read `references/camera-raw-real-estate-guide.md` before giving final slider values.

## Required Output Format

Respond in Brazilian Portuguese. Use parameter names exactly as they appear in Adobe Camera Raw PT-BR. Always provide exact values.

When the user sends two or more images, first decide whether they belong to the same project, room, facade, view, or lighting condition. If they should match in a video, add a short `BASE DE COR DO PROJETO` section before individual prescriptions, explaining the shared color direction and which sliders must stay consistent.

### DIAGNÓSTICO DA IMAGEM

Write 3-5 sentences describing lighting condition, color issues, texture/material issues, AI artifacts if present, and the edit goal.

### CONFIGURAÇÕES CAMERA RAW

#### Painel: Luz

| Parâmetro | Valor | Justificativa |
| --- | ---: | --- |
| Exposição |  |  |
| Contraste |  |  |
| Realces |  |  |
| Sombras |  |  |
| Brancos |  |  |
| Pretos |  |  |

#### Painel: Cor

| Parâmetro | Valor | Justificativa |
| --- | ---: | --- |
| Temperatura |  |  |
| Colorir |  |  |
| Vibração |  |  |
| Saturação |  |  |

#### Painel: Efeitos

| Parâmetro | Valor | Justificativa |
| --- | ---: | --- |
| Textura |  |  |
| Claridade |  |  |
| Desembaçar |  |  |
| Vinheta |  |  |
| Granulado |  |  |

#### Painel: Curva (Paramétrica)

| Parâmetro | Valor | Justificativa |
| --- | ---: | --- |
| Realces |  |  |
| Claros |  |  |
| Escuros |  |  |
| Sombras |  |  |

#### Painel: Misturador de Cores - HSL

Only include color channels that need adjustment. Omit channels that remain 0/0/0.

| Canal | Matiz | Saturação | Luminescência | Justificativa |
| --- | ---: | ---: | ---: | --- |

### AJUSTES LOCAIS / MÁSCARAS

Include only when needed. Mention masks for sky, windows, walls/ceiling, greenery, water, facade/materials, people/skin, or interior shadows.

### RESUMO

End with exactly one line:

`Perfil aplicado: [tipo de cena]. Edição cinematográfica realista.`

## Photoshop 2026 Handoff

When the user mentions Photoshop 2026, frame the recommendations as `Filtro > Filtro do Camera Raw` settings:

1. Prefer editing a Smart Object/non-destructive layer.
2. Start with `Luz`, then `Cor`, then `Efeitos`, then `Curva`, then `Misturador de cores`.
3. Recheck the image at fit-to-screen and 100 percent zoom.
4. If the image is severely degraded by blur, banding, smearing, or broken geometry, state that Camera Raw alone will not solve it and suggest regeneration or retouching.
