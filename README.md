# Dashboard JSC

Página independente do repositório projetotim. Fonte: cópia local de Manual_TIM_JSC_Rollout.xlsx, aba Manual.

- Botões de Projeto (coluna B) e UF (coluna D), combinados entre si.
- Somente registros cuja coluna V (SUB MANUAL) contém JSC, sem distinguir maiúsculas e minúsculas.
- Indicadores, gráficos e tabela acompanham os filtros.
- A base é uma fotografia da planilha; não existe sincronização automática com o OneDrive.

## Publicação no GitHub Pages

Crie um repositório separado e envie index.html, dashboard-data.js e .nojekyll para a raiz. Em Settings > Pages, selecione Deploy from a branch, a branch main e a pasta /(root). O GitHub informará o endereço publicado.

Os dados incluídos em dashboard-data.js ficam disponíveis a quem acessar a página publicada.

## Atualização da base

Com Python e openpyxl instalados, defina DASHBOARD_SOURCE com o caminho do arquivo Excel e execute scripts/atualizar-dados.py. Publique novamente dashboard-data.js após atualizar. A planilha original não é modificada. As fórmulas são lidas a partir dos valores salvos no Excel.
