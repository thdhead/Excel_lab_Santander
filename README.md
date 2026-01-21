# Excel_lab_Santander

1) Visão geral do projeto
Este projeta implementa um dashboard de vendas (base fictícia) para assinaturas do Xbox Game Pass, com foco em:
Receita (Total Value)
Separação de visualização por Subscription Type: Monthly / Quarterly / Annual
Segmentação por Auto Renewal (Yes/No)
KPIs de receita dos add-ons: EA Play Season Pass Price e Minecraft Season Pass Price

2) Estrutura do arquivo (abas)
A̳ssets
Paleta de cores, logos e ícones usados para padronizar o visual do dashboard.
B̳ases
Base de dados com os registros de assinantes e valores monetários que alimentam os pivôs.
C̳álculos
Área de PivotTables (tabelas dinâmicas) que agregam os dados e servem de fonte para:
Gráficos do dashboard
D̳ashboard
Área final de visualização com:
KPIs (Minecraft e EA)
Gráfico(s) por Subscription Type e Auto Renewal
Segmentações via slicers

4) Dados utilizados (colunas da base)
A base está na aba B̳ases com as colunas:

Subscriber ID — identificador do assinante
Name — nome do assinante
Plan — plano (ex.: Core / Standard / Ultimate)
Start Date — data de início
Auto Renewal — renovação automática (Yes/No)
Subscription Price — preço da assinatura
Subscription Type — periodicidade (Monthly / Quarterly / Annual)
EA Play Season Pass — indicador (Yes/No)
EA Play Season Pass Price — valor do EA Play
Minecraft Season Pass — indicador (Yes/No)
Minecraft Season Pass Price — valor do Minecraft
Coupon Value — valor de cupom/desconto
Total Value — valor total do cliente (medida principal de receita)

4) O que foi construído (transformações e análises)
Criação de PivotTables na aba C̳álculos para:
Agregar Total Value por Subscription Type e Auto Renewal
Somar valores de add-ons (EA e Minecraft)
Contagens por Plan (para visão de base de clientes)
No D̳ashboard, os KPIs de EA e Minecraft são puxados por fórmulas ligadas aos pivôs.

5) Como reproduzir (passo a passo)
Abra o arquivo excel_lab.xlsx no Excel 365.
Valide os dados, normalize os valores.
Valide que os dados estão consistentes.
Vá até a aba B̳ases e substitua/adicione linhas na tabela mantendo:
Os mesmos nomes de colunas
O mesmo tipo de dado
Crie os pivot tables
Atualize os pivots:
Vá para a aba D̳ashboard e use os slicers para filtrar:
Verifique que:
KPIs (EA e Minecraft) mudam com os filtros
Gráficos refletem os mesmos filtros aplicados
