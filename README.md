# novo-aula-Rafael

Este repositório inclui as 9 skills de marketing para Instagram do projeto
[sergebulaev/instagram-skills](https://github.com/sergebulaev/instagram-skills)
(licença MIT, commit `652be40`), instaladas como skills de projeto do Claude Code.

## Skills disponíveis (`.claude/skills/`)

| Skill | Para que serve |
|---|---|
| `ig-caption-writer` | Legendas com gancho nos primeiros 125 caracteres |
| `ig-carousel-planner` | Planejamento de carrossel slide a slide |
| `ig-hook-extractor` | Extrai e classifica ganchos de Reels/carrosséis virais |
| `ig-hashtag-strategist` | Estratégia e dimensionamento de hashtags |
| `ig-humanizer` | Remove "cara de IA" e faz auditoria antes de publicar |
| `ig-repurposer` | Adapta conteúdo de outras redes para o Instagram |
| `ig-profile-optimizer` | Otimização de bio e perfil |
| `ig-audience-insights` | Análise de nicho/perfil com dados reais (Apify) |
| `ig-content-planner` | Calendário semanal de Reels, carrosséis e stories |

Basta abrir o Claude Code nesta pasta e pedir, por exemplo:
"Escreva uma legenda para este Reel sobre ..." — a skill certa é ativada automaticamente.

## Integrações opcionais

As skills funcionam só com rascunhos, sem nenhuma chave. Para publicar,
gerar imagens ou ler dados reais, copie `.env.example` para `.env`
(já ignorado pelo git) e preencha `PUBLORA_API_KEY`, `APIFY_TOKEN` ou
`PIXFARO_TOKEN`, e instale as dependências com `pip install -r requirements.txt`.

## Estrutura

- `.claude/skills/` — as 9 skills
- `.claude/references/` — referências compartilhadas (fórmulas de gancho, hashtags, voz)
- `lib/` — clientes Python (Publora, Apify, Pixfaro, parser de URL)
- `scripts/` — verificações do pacote original
