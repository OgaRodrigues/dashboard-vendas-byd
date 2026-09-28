# 📊 Dashboard de Vendas - BYD Brasil (2024-2026)

## 📌 Visão Geral do Projeto
Este projeto consiste no desenvolvimento de um dashboard interativo em Power BI para analisar o histórico interno de emplacamentos da BYD no mercado brasileiro, cobrindo o período de janeiro de 2024 a agosto de 2026. 

O objetivo principal foi transformar dados brutos de registros de vendas em uma solução analítica visual, permitindo a extração de insights estratégicos sobre o desempenho de modelos e tipos de motorização da própria marca.

---

## 💡 Perguntas de Negócio Respondidas
* **Concentração de Vendas:** Qual o peso do modelo *Dolphin Mini* no faturamento físico da marca? O painel demonstra o isolamento do modelo no topo do ranking interno.
* **Mix de Tecnologias:** O consumidor interno da marca demonstra preferência por veículos *100% Elétricos* ou *Híbridos Plug-in*? O relatório revela um equilíbrio próximo a 50/50 entre as tecnologias.
* **Volume Acumulado:** Qual o total de vendas que sustenta essa trajetória? O KPI principal destaca o marco de 281 Mil unidades.

---

## 🛠️ Detalhes Técnicos e Arquitetura

### 1. Processo de ETL (Extração e Limpeza)
* **Origem:** Dados extraídos de informativos de emplacamentos (Fenabrave/ABVE) unificados em arquivo estruturado `.csv`.
* **Tratamento (Power Query):** 
  * Conversão de tipos de dados e padronização da coluna cronológica.
  * Configuração de localidade regional para garantir a integridade da leitura temporal em conformidade com o calendário brasileiro.

### 2. Design e UI (Interface do Usuário)
* **Identidade Visual:** Aplicação de paleta de cores baseada no branding institucional da BYD (Cinza Grafite `#4A525A` como plano de fundo e Azul Elétrico `#007ACC` para destaque de métricas).
* **Elementos Visuais:** Utilização de contêineres transparentes com efeitos de profundidade (*Drop Shadow*) e bordas arredondadas para simular cartões flutuantes.

### 3. Filtros Dinâmicos (UX)
* **Segmentação Eficiente:** Implementação de um Segmentador Horizontal (*Tile Slicer*) por Ano, evitando a necessidade de Bookmarks complexos e mantendo a alta performance e leveza do relatório (`.pbix`).
