# ⛽ Análise dos Preços de Combustíveis no Brasil

<p>
  <img src="https://img.shields.io/badge/Python-3.14-3776AB?logo=python&logoColor=white" alt="Python 3.14">
  <img src="https://img.shields.io/badge/Dados-ANP-17365D" alt="Dados da ANP">
  <img src="https://img.shields.io/badge/SQL-DuckDB-FFF000?logo=duckdb&logoColor=black" alt="DuckDB">
  <img src="https://img.shields.io/badge/Ambiente-uv-DE5FE9" alt="uv">
</p>

> Projeto de portfólio em desenvolvimento para explorar a série histórica de preços de combustíveis divulgada pela Agência Nacional do Petróleo, Gás Natural e Biocombustíveis (ANP).

O objetivo é organizar os dados e construir uma análise reprodutível que ajude a descrever como os preços pesquisados variam entre períodos, produtos e localidades. As conclusões serão limitadas ao escopo e à cobertura da pesquisa: um preço atípico, por si só, não demonstra irregularidade, e os registros não devem ser tratados como um censo de todos os postos.

## 🎯 Perguntas que a análise vai explorar

- Como os preços pesquisados variam ao longo do tempo?
- Como se distribuem por produto e localidade?
- Quais diferenças e limitações precisam ser consideradas ao comparar esses grupos?

Os resultados e as perguntas serão refinados à medida que o dicionário e a qualidade dos dados forem estudados.

## 🧭 Etapas do projeto

1. **Entender os dados:** documentar as colunas, unidades, período e cobertura; verificar qualidade e limitações.
2. **Consultar com SQL:** preparar consultas e tabelas resumidas com DuckDB.
3. **Explorar e comunicar:** usar Python para análise descritiva, visualizações e conclusões com ressalvas.
4. **Apresentar os resultados:** publicar um dashboard e documentar como reproduzir a análise.

## 🛠️ Tecnologias

- **Python** para análise e automação.
- **pandas** e **PyArrow** para manipulação de dados.
- **DuckDB** para consultas SQL locais.
- **Matplotlib** e **Seaborn** para visualizações.
- **Jupyter** para exploração documentada.
- **uv** para gerenciar dependências e o ambiente do projeto.

## 📁 Organização

```text
├── app/          # aplicação (etapa futura)
├── dashboard/    # dashboard (etapa futura)
├── data/
│   └── raw/      # dados de origem; arquivos locais não são versionados
├── docs/         # documentação e decisões
├── notebooks/   # exploração documentada
├── sql/          # consultas SQL
├── src/          # código reutilizável
└── tests/        # verificações automatizadas
```

## 🚀 Como começar

Pré-requisitos: Python 3.14 e [uv](https://docs.astral.sh/uv/).

```bash
uv sync
uv run python --version
```

O `uv sync` instala as dependências registradas no projeto e prepara o ambiente virtual local. Para executar um script ou ferramenta, use `uv run`, por exemplo:

```bash
uv run jupyter lab
```

## 📊 Dados e cuidados

Os dados são da pesquisa de preços de combustíveis da ANP. O arquivo original deve ser preservado sem alterações. Dados brutos locais ficam em `data/raw/` e não devem ser enviados ao Git; consulte a documentação oficial da ANP para entender metodologia, período e cobertura antes de interpretar resultados.

Este repositório está no início da trilha: dicionário de dados, perfil de qualidade, consultas, análises e dashboard serão adicionados conforme forem concluídos. Por isso, este README ainda não apresenta resultados nem afirma impactos que não foram medidos.

## 📌 Status

**Fase 0 — preparação do projeto.** Próxima entrega: compreender e documentar os dados.

