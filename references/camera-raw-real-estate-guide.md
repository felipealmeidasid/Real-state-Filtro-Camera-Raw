# Camera Raw Archviz and Real Estate Guide

Use these values as expert starting guidance for Adobe Camera Raw Filter in Photoshop 2026. The final response must give exact slider values. Judge the image first; do not apply recipes blindly.

Default style: cinematic realistic real estate photography. The image should feel professional, dimensional, and premium, while avoiding blown-out color, neon vegetation, electric skies, plastic materials, and other common AI-generation tells.

## Exact Values Policy

- Always output one exact value per setting, such as `Realces -35`, not `-25 to -45`.
- Use the ranges below only as internal decision bands.
- If uncertainty is high because the image is compressed, low resolution, or partially obscured, still choose an exact value and mention the uncertainty in the justification.
- For multiple images from the same project, prioritize matched color over individually dramatic edits.

## Parameter Ranges

- Luz: Exposição -5.00 to +5.00; Contraste, Realces, Sombras, Brancos, Pretos -100 to +100.
- Cor: Temperatura, Colorir, Vibração, Saturação -100 to +100.
- Efeitos: Textura, Claridade, Desembaçar, Vinheta -100 to +100; Granulado 0 to +100.
- Curva paramétrica: Realces, Claros, Escuros, Sombras -100 to +100.
- Misturador de Cores HSL: Matiz, Saturação, Luminescência -100 to +100 per channel.

## Professional Evaluation Checklist

Assess each image through these lenses before prescribing values.

### Architectural Photographer

- Lighting condition: golden hour, blue hour, overcast, midday harsh sun, interior artificial, mixed light, night.
- Dynamic range: blown highlights, crushed shadows, flat histogram, overly even CGI lighting.
- Exposure: underexposed, overexposed, centered, artificially bright, or too dense for marketing.
- White balance: yellow/orange interior cast, blue/cyan exterior cast, green/magenta shift, mixed light conflict.
- Architectural readability: facade shape, material separation, depth, window detail, and room spaciousness.

### Colorist

- Dominant and secondary palettes: neutrals, wood, greenery, sky, water, warm lamps, concrete, stone, metal.
- Color contamination: AI color bleeding, synthetic saturation zones, orange tungsten exaggeration, neon greens, electric blues/cyans.
- Skin tone accuracy if people are present.
- Sky, water, vegetation, and glass fidelity.
- AI tells: oversaturated accents, plastic materials, uniform color fields, perfect blacks, too-clean whites.

### Retoucher

- Sharpness versus AI softness, especially in Seedance/Kling/video stills.
- AI artifacts: smearing, repeated texture, warped detail, banding, muddy edges, unnatural smooth surfaces.
- Material realism: glass, concrete, wood, metal, water, fabric, landscaping.
- Atmospheric depth: haze/fog that helps realism versus haze that looks like low contrast.
- Noise and grain: archviz normally needs clean output, not film grain.

## Hard Rules

1. Claridade must be 0 for scenes with human skin or prominent water. Positive Claridade makes skin artificial and water edges harsh.
2. Do not adjust Temperatura or Desembaçar in golden hour/sunset scenes unless the image is clearly broken. Preserve the natural warm atmospheric cast.
3. Granulado must be 0 for archviz and real estate by default. Use Granulado +8 only for automotive close-ups, if the user explicitly needs that style.
4. Keep values conservative by default. Preferred range for most sliders is -30 to +30; go beyond only with a clear reason.
5. Use strong negative Realces only when the image has real highlight stress: sun, sky, lamps, LEDs, windows, white facades, wet pavement reflections, or clipped-looking clouds. For normal daylight without highlight stress, prefer -15 to -35; reserve -40 to -60 for clearly bright or blown areas.
6. Use high Textura only when it improves believable material detail: aerials, maquettes, construction sites, stone, roof tiles, asphalt, facade texture, landscaping, or product/material close-ups. Keep Textura 0 to +10 for skin, water, rain, glass, smooth walls, clean skies, and soft atmospheric scenes.
7. Never push Saturação above +15 for archviz or AI-generated real estate images. Prefer Vibração for a controlled lift.
8. For archviz exteriors, Pretos should not go below -20. Crushed blacks destroy facade and landscaping detail.
9. Desembaçar max +20 for interiors and aerials. Use 0 for exteriors with sky unless haze is the main flaw; Dehaze can shift sky color and create unnatural cloud contrast.
10. Vinheta should be 0 for standard real estate output. Use only negative values from -5 to -15 for editorial/magazine style. Never use positive vinheta.
11. In HSL Azuis, never increase Saturação on sky. AI skies are often already oversaturated; reduce saturation or adjust Luminescência instead.
12. Curva adjustments should be gentle, normally within ±15. The Curva panel fine-tunes after Luz does the main work; large curve moves create banding in AI gradients.
13. If people are visible, preserve natural skin first. Avoid global color moves that make skin orange, magenta, gray, or waxy.
14. If the image has visible banding, heavy smearing, broken geometry, or severe blur, state that Camera Raw alone cannot fully fix it.

## Grading Profiles by Scene Type

### Exterior Diurno

Goal: cinematic realistic daylight with clean facade detail, controlled sky, and no heavy HDR.

| Panel | Bias |
| --- | --- |
| Luz | Exposição +0.05 to +0.25; Contraste +5 to +15; Realces -20 to -45; Sombras +10 to +30; Brancos 0 to +15; Pretos -5 to -18. |
| Cor | Temperatura -5 to +3 if needed; Colorir -3 to +5; Vibração +5 to +12; Saturação -5 to +5. |
| Efeitos | Textura +10 to +20; Claridade +3 to +10; Desembaçar 0 if sky is present, +5 to +10 only for mild haze; Vinheta 0. |
| Curva | Gentle S-curve: Realces +3 to +8, Claros +2 to +6, Escuros -2 to -8, Sombras -2 to -8. |
| HSL | Verdes Saturação -5 to -20, Luminescência +5 to +15; Azuis Saturação 0 to -15, Luminescência -5 to +10 depending sky brightness. |

### Exterior Golden Hour / Sunset

Goal: warm cinematic atmosphere without AI orange overload or clipped highlights.

| Panel | Bias |
| --- | --- |
| Luz | Exposição -0.30 to +0.05; Contraste +5 to +15; Realces -30 to -60; Sombras +20 to +40; Brancos -10 to +5; Pretos -5 to -15. |
| Cor | Temperatura 0; Colorir 0 unless magenta/green cast is obvious; Vibração 0 to +5; Saturação -5 to +3. |
| Efeitos | Textura +5 to +15; Claridade 0 to +8 if no skin/water; Desembaçar 0; Vinheta -5 to -12 only for editorial output. |
| Curva | Keep within ±10. Preserve smooth sky gradients. |
| HSL | Laranjas Saturação -10 to -20; Amarelos Saturação -5 to -15; Azuis do sky: Saturação 0 to -15, not positive. |

### Exterior Noturno / Blue Hour

Goal: moody, luxurious, cinematic, and controlled artificial lighting.

| Panel | Bias |
| --- | --- |
| Luz | Exposição +0.20 to +0.50; Contraste +10 to +20; Realces -20 to -45; Sombras +10 to +30; Brancos 0 to +10; Pretos -5 to -18. |
| Cor | Temperatura -5 to -10 if the image is too yellow; Colorir -3 to +5; Vibração +5 to +12; Saturação -5 to +5. |
| Efeitos | Textura +8 to +18; Claridade +8 to +12 if no skin/water; Desembaçar 0 to +8; Vinheta -8 to -12 for editorial luxury. |
| Curva | Slight contrast only, within ±12. |
| HSL | Azuis Luminescência +10 to +20 for controlled blue hour; Laranjas/Amarelos Saturação -5 to -15 if artificial lights are too strong. |

### Interior Luz Natural

Goal: airy, clean, spacious, cinematic realistic interior photography.

| Panel | Bias |
| --- | --- |
| Luz | Exposição +0.10 to +0.30; Contraste 0 to +10; Realces -20 to -45; Sombras +20 to +40; Brancos -10 to +5; Pretos -5 to -15. |
| Cor | Temperatura +3 to +8 when too cold; reduce if walls are yellow; Colorir 0 to +6 to counter green casts; Vibração +3 to +10; Saturação -5 to +3. |
| Efeitos | Textura +10 to +25 for materials; Claridade 0 to +5; Desembaçar 0 to +5; Vinheta 0; Granulado 0. |
| Curva | Lift clarity gently: Claros +3 to +8, Sombras -2 to -6. |
| HSL | Amarelos Saturação -5 to -15 for wood/wall exaggeration; Laranjas Saturação -5 to -12 if wood is too orange. |

### Interior Luz Artificial

Goal: warm, inviting, cinematic, controlled, without exaggerated tungsten orange.

| Panel | Bias |
| --- | --- |
| Luz | Exposição 0 to +0.25; Contraste +3 to +12; Realces -20 to -50 for lamps; Sombras +15 to +30; Brancos -10 to +5; Pretos -5 to -15. |
| Cor | Correct white balance first: Temperatura -5 to -15 if too warm, +3 to +8 if sterile; Colorir +2 to +8 if green cast exists; Vibração +3 to +8; Saturação -5 to +3. |
| Efeitos | Textura +8 to +20; Claridade 0 to +5; Desembaçar 0; Vinheta 0. |
| Curva | Small contrast, ±10 max. |
| HSL | Laranjas and Amarelos Saturação -10 to -20 when lights/wood look AI-orange. |

### Aerial / Drone View

Goal: cinematic scale, clean detail, controlled haze, and believable landscape color.

| Panel | Bias |
| --- | --- |
| Luz | Exposição 0 to +0.20; Contraste +15 to +25; Realces -30 to -50; Sombras +5 to +25; Brancos +5 to +15; Pretos -10 to -20. |
| Cor | Temperatura -5 to +3; Colorir -3 to +5; Vibração +5 to +12; Saturação -5 to +5. |
| Efeitos | Textura +20 to +30; Claridade +10 to +15 if people/skin are not visible; Desembaçar +8 to +15; Vinheta 0. |
| Curva | Gentle S-curve within ±12. |
| HSL | Verdes Saturação -10 to -20; Verdes Luminescência +5 to +15; Azuis Saturação 0 to -15. |

### Piscina / Água em Destaque

Goal: clear water, believable color, smooth surface, and premium resort-like realism.

| Panel | Bias |
| --- | --- |
| Luz | Exposição 0 to +0.20; Realces -20 to -45; Sombras +5 to +25; Brancos -5 to +10; Pretos -5 to -15. |
| Cor | Temperatura neutral to slightly cool if water is yellow; Vibração 0 to +8; Saturação -5 to +3. |
| Efeitos | Textura 0 to +5; Claridade 0; Desembaçar 0 to +5; Vinheta 0; Granulado 0. |
| Curva | Very gentle, within ±8. |
| HSL | Águas Saturação -5 to -15, Luminescência +10 to +15; Azuis Saturação 0 to -10, Luminescência +5 to +15. |

### Render Muito Sintético

Goal: reduce CGI tells while preserving cinematic commercial polish.

| Panel | Bias |
| --- | --- |
| Luz | Exposição -0.10 to +0.15; Contraste -5 to +8; Realces -10 to -35; Sombras +5 to +25; Brancos -5 to +10; Pretos 0 to -12. |
| Cor | Temperature/tint only to remove obvious cast; Vibração 0 to +8; Saturação -8 to 0. |
| Efeitos | Textura -5 to +10 depending material realism; Claridade -5 to +5; Desembaçar 0; Vinheta 0. |
| Curva | Minimal curve, within ±8. |
| HSL | Reduce only offending synthetic channels: usually Verdes, Azuis, Águas, Laranjas, or Amarelos. |

## Color Mixer Targets

- Vermelhos: reduce Saturação -5 to -20 when brick, decor, sunset, or wood pulls too much attention.
- Laranjas: reduce Saturação -5 to -20 for orange wood, tungsten light, skin over-warmth, or sunset overload. Adjust Luminescência +5 to +15 for cleaner interiors.
- Amarelos: reduce Saturação -5 to -20 for yellow walls, warm floors, lamps, and grass contamination. Shift Matiz slightly negative/positive only if the hue is visibly wrong.
- Verdes: reduce Saturação -5 to -25 when vegetation is neon; Luminescência +5 to +20 for fresh but realistic landscaping.
- Águas: reduce Saturação -5 to -15 for cyan pools/glass; Luminescência +5 to +15 for cleaner water.
- Azuis: never increase sky Saturação; use Saturação 0 to -20 and Luminescência -10 to +20 to control depth/brightness.
- Violetas/Magentas: usually leave at 0 unless AI creates magenta contamination in lights, sky gradients, or decor.

## Local Masks

| Mask | Typical Adjustments | Purpose |
| --- | --- | --- |
| Céu | Realces -20 to -70, Brancos -10 to -30, Desembaçar 0 to +8, Saturação -5 to 0 | Recover sky detail without making it electric or crunchy. |
| Janelas | Exposição -0.20 to -0.80, Realces -40 to -100, Brancos -10 to -40 | Recover exterior view without dulling the room. |
| Paredes/Teto | Temperatura/Colorir correction, Saturação -5 to -15, Textura -5 to +5 | Clean color casts while preserving material softness. |
| Vegetação | Saturação -5 to -25, Luminescência +5 to +20, small Matiz correction | Avoid neon green AI landscaping. |
| Água | Claridade 0, Textura 0 to +5, Águas Saturação -5 to -15, Luminescência +10 to +15 | Keep pools/water clean and smooth. |
| Fachada/Materiais | Textura +5 to +15, Claridade +3 to +10, Realces -10 to -35 | Reveal material quality and architectural shape. |
| Pessoas/Pele | Claridade 0, Textura -5 to +5, Saturação conservative, Colorir carefully | Avoid waxy or oversharp skin. |
| Sombras internas | Sombras +10 to +35, Pretos 0 to -10, Redução de Ruído +5 to +20 | Reveal detail without gray blacks. |

## Detail, Optics, and Geometry

- Sharpening for architecture: Amount 30-60, Radius 0.7-1.2, Detail 15-35, Masking 40-80.
- Noise Reduction: Luminance 5-25, Color 20-30; higher for night/dusk, lower for clean renders.
- Enable profile corrections and remove chromatic aberration when editing real photos.
- Correct verticals for architecture, but avoid extreme geometry correction that distorts rooms or facades.

## Batch Consistency for Real Estate Video

1. Group images by project area and lighting: same room, same facade, same view, day interior, day exterior, dusk, night, amenity, aerial.
2. Choose the strongest image in each group as the hero reference.
3. Build one base grade per group. Keep Temperatura, Colorir, Contraste, Vibração, Saturação, HSL greens, HSL blues, and black point aligned across the group.
4. Use per-image exceptions only for exposure, highlight recovery, shadow opening, masks, and artifact correction.
5. If two images are the same room or same exterior view, do not make one warmer/cooler or more saturated unless the lighting visibly changed.
6. Keep sky blue, vegetation green, wall neutrality, water color, wood warmth, and black point consistent across consecutive shots.
7. Review the images as a contact sheet or timeline sequence before final export to catch color jumps.

## Multi-Image Response Guidance

When multiple images are analyzed together, structure the answer as:

1. `BASE DE COR DO PROJETO`: one short paragraph defining shared cinematic realistic direction.
2. Shared settings table when all images can use the same base grade.
3. `AJUSTES POR IMAGEM`: exact exceptions for each image.
4. Consistency note for video: what must remain identical across the sequence.
