# Demonstração do SafeWay

## Visão Geral

O SafeWay é uma aplicação web completa para predição de acidentes de trânsito, desenvolvida com FastHTML e inspirada no design moderno da imagem de referência fornecida.

## Funcionalidades Implementadas

### 1. Dashboard Principal
- **Cards de Estatísticas**: Exibem métricas importantes como número de acidentes, precisão do modelo, predições realizadas e alertas ativos
- **Mapa de Calor**: Visualização interativa dos acidentes por região usando Folium
- **Gráficos Dinâmicos**: 
  - Acidentes por horário (gráfico de barras)
  - Tendência dos últimos 30 dias (gráfico de linha)
  - Distribuição por condições meteorológicas (gráfico de pizza)
  - Ranking de estados (gráfico de barras horizontal)

### 2. Sistema de Predição
- **Formulário Intuitivo**: Campos para data, horário, UF, município e condições meteorológicas
- **Seleção Dinâmica**: Municípios são carregados automaticamente baseados na UF selecionada
- **Modelo de ML Integrado**: Utiliza o modelo original do repositório com melhorias
- **Resultado Detalhado**: Mostra probabilidade, nível de risco e descrição

### 3. Design e Interface
- **Layout Responsivo**: Baseado no design da imagem SafeWay fornecida
- **Sidebar de Navegação**: Com ícones e indicação da página ativa
- **Header Informativo**: Mostra informações do usuário
- **Tema Consistente**: Cores azuis (#4A90E2, #2C5282) e design moderno

## Tecnologias Utilizadas

- **FastHTML**: Framework web moderno para Python
- **Bootstrap 5**: Framework CSS para design responsivo
- **Plotly.js**: Biblioteca para gráficos interativos
- **Folium**: Mapas interativos com Leaflet
- **LightGBM**: Modelo de machine learning para predições
- **Pandas/NumPy**: Manipulação e análise de dados

## Estrutura de Arquivos

```
safeway-predicao/
├── app.py                    # Aplicação principal
├── prediction.py             # Módulo de predição
├── dashboard.py              # Módulo do dashboard
├── data_generator.py         # Gerador de dados simulados
├── model_integration.py      # Integração com ML
├── preditor_ofc.py          # Modelo original
├── *.json                   # Dados de UFs, municípios e clima
├── requirements_simple.txt  # Dependências
└── README.md               # Documentação
```

## Como Usar

1. **Instalar dependências**: `pip install -r requirements_simple.txt`
2. **Executar aplicação**: `python3 app.py`
3. **Acessar**: `http://localhost:5001`

## Páginas Disponíveis

- `/` - Dashboard principal com visualizações
- `/prediction` - Formulário de predição
- `/reports` - Relatórios (placeholder)
- `/settings` - Configurações (placeholder)

## Características Técnicas

- **Responsivo**: Funciona em desktop, tablet e mobile
- **Interativo**: Gráficos e mapas interativos
- **Performático**: Carregamento rápido e otimizado
- **Modular**: Código organizado em módulos separados
- **Extensível**: Fácil de adicionar novas funcionalidades

O projeto demonstra uma implementação completa e profissional de um sistema de predição de acidentes, combinando design moderno, funcionalidades avançadas e integração com machine learning.
