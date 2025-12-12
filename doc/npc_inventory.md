# NPC Script Inventory and Initial Scope

## Diretórios principais em `npc/`
- **cities**: scripts por cidade (ex.: `prontera.txt`, `geffen.txt`, `morocc.txt`).
- **kafras**: serviços de Kafra e warpers principais (`kafras.txt`, `dts_warper.txt`, `cool_event_corp.txt`, `functions_kafras.txt`).
- **merchants**: vendedores e serviços de refino/dye/etc. (ex.: `refine.txt`, `shops.txt`, `socket_enchant.txt`).
- **warps**: warps organizados por tipo: `cities/`, `dungeons/`, `fields/`, `other/`, além de `guildcastles.txt` e `pvp.txt`.
- **quests**: quests principais e subdivisões (`quests_prontera.txt`, `quests_geffen.txt`, subpastas `newgears/`, `first_class/`, `skills/`, `seals/`).

## Inventário de scripts prioritários
- **`npc/cities/prontera.txt`** – NPCs gerais de Prontera (guards, guias de história, diálogos de novato). Útil para validação de comportamento base da capital.【F:npc/cities/prontera.txt†L1-L37】
- **`npc/kafras/kafras.txt`** – Implementação padrão dos serviços de Kafra (salvar ponto, storage, carrinho) com parametrização por chamada de função `F_Kafra`. Essencial para checar tarifas e mensagens oficiais.【F:npc/kafras/kafras.txt†L1-L37】
- **`npc/kafras/dts_warper.txt`** – Warper de Dungeon Teleport Service; cobre teleporte pago para mapas chave (prioridade secundária para rotas iniciais).
- **`npc/warps/cities/prontera.txt`** – Warps internos de Prontera e conexões para campos e interiores (referência principal para mobilidade da capital).【F:npc/warps/cities/prontera.txt†L1-L37】
- **`npc/quests/quests_prontera.txt`** – Conjunto de quests de Prontera: acesso ao Culvert, quest do chapéu Ph.D, Geoborg Family Curse, e hooks para Nameless Island. Serve de base para quests urbanas iniciais.【F:npc/quests/quests_prontera.txt†L1-L24】
- **`npc/quests/quests_geffen.txt`** – Quests urbanas de Geffen (seguinte prioridade após Prontera).
- **`npc/warps/cities/geffen.txt`** – Warps de Geffen (para continuidade do eixo capital → cidades mágicas).
- **`npc/merchants/refine.txt`** e **`npc/merchants/shops.txt`** – Serviços de refino e vendedores padrão acessados cedo pelos jogadores.

## Escopo inicial proposto
1. **Capital (Prontera)**
   - Verificar serviços de Kafra padrão (`npc/kafras/kafras.txt`).
   - Auditar warps principais de cidade/campo (`npc/warps/cities/prontera.txt`).
   - Revisar quests urbanas críticas (`npc/quests/quests_prontera.txt`).
2. **Cidade secundária imediata: Geffen**
   - Warps urbanos (`npc/warps/cities/geffen.txt`).
   - Quests de cidade (`npc/quests/quests_geffen.txt`).
3. **Serviços transversais**
   - Vendedores essenciais (`npc/merchants/refine.txt`, `npc/merchants/shops.txt`).
   - Warper DTS para rotas pré-renewal (`npc/kafras/dts_warper.txt`).

O foco inicial concentra-se na capital e conexões diretas; áreas menores ou temáticas (dungeons específicas, eventos sazonais) entram em fases posteriores.
