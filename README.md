# Excel_lab_Santander

# excel_lab.xlsx — Dashboard de Vendas (Xbox Game Pass)

## Objetivo
Esta planilha organiza e analisa uma base fictícia de assinaturas do Xbox Game Pass e add-ons (EA Play e Minecraft), usando Tabela do Excel + Tabelas Dinâmicas para gerar métricas e um dashboard com gráficos.

## Estrutura do arquivo (abas)
- **Dashboard**
  - Painel com título, elementos visuais e gráficos (barra e pizza).
  - Indicadores puxados por fórmulas **GETPIVOTDATA** (ex.: totais de Minecraft Season Pass e EA Play).

- **Cálculos**
  - Área com **Tabelas Dinâmicas** que alimentam o Dashboard, incluindo:
    - Soma de **Total Value** (receita total) por categoria (ex.: renovação).
    - Soma de valores de add-ons (Minecraft e EA Play).
    - Contagem/distribuição por plano (**Core/Standard/Ultimate**).

- **Bases**
  - Base principal em uma **Tabela do Excel (Tabela1)** com colunas como:
    - Subscriber ID, Name, Plan, Start Date, Auto Renewal
    - Subscription Price, Subscription Type
    - EA Play Season Pass (+ Price)
    - Minecraft Season Pass (+ Price)
    - Coupon Value, Total Value
  - Essa tabela é a fonte das Tabelas Dinâmicas.

- **Assets**
  - Paleta de cores (hex) e imagens/elementos usados para padronizar o visual do Dashboard.

## Principais métricas/visões
- Receita total (**Total Value**) consolidada e segmentada (via Tabela Dinâmica).
- Distribuição por plano (Core/Standard/Ultimate).
- Totais de add-ons (EA Play e Minecraft) exibidos no Dashboard via **GETPIVOTDATA**.

## Como usar / atualizar
1. Abra `excel_lab.xlsx` no Microsoft Excel.
2. Atualize tudo: **Dados > Atualizar Tudo** (para recalcular Tabelas Dinâmicas e o Dashboard).
3. Use filtros/slicers (quando disponíveis) para segmentar as visões.
4. Para adicionar novos registros:
   - Insira novas linhas dentro da **Tabela1** na aba **Bases**;
   - Depois execute **Atualizar Tudo** novamente.

## Observações
- O Dashboard depende de Tabelas Dinâmicas e **GETPIVOTDATA** (em Google Sheets pode não funcionar igual).
- Se renomear colunas/campos, revise as Tabelas Dinâmicas e as fórmulas no Dashboard.
