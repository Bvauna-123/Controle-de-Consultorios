# Código-fonte — Gerenciador de Consultórios Personal Cariacica

Esta cópia corresponde à versão publicada do sistema em 28/09/2026. Inclui interface, API, esquema e migrações do banco D1, e o arquivo de importação da planilha de setembro a dezembro de 2026.

## Estrutura principal
- app/page.tsx: tela de ocupação semanal e impressão A4 horizontal.
- app/api/bookings/route.ts: consulta, cadastro e exclusão de ocupações.
- lib/import.ts e data/import-2026.json: importação inicial e anotações para conferência.
- db/schema.ts e drizzle/: estrutura e migrações do banco.

## Para desenvolver
Requer Node.js 22 ou superior. Instale as dependências com `pnpm install` e use `pnpm dev`. A persistência usa Cloudflare D1 com o binding `DB`; para uma implantação independente, configure seu próprio projeto e banco. O arquivo `.openai/hosting.json` contém o ID do Site original: não publique uma cópia usando esse mesmo ID por engano.

O ZIP contém o código e os dados de origem da importação, mas não uma exportação dos registros atuais do banco de produção.
