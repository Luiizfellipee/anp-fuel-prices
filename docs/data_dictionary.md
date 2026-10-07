### Dicionário inicial

| Campo | Uso no projeto | Cuidado |
|---|---|---|
| `Regiao - Sigla` | Região (N, NE, CO, SE, S) | Texto |
| `Estado - Sigla` | UF | Texto |
| `Municipio` | Município | Sem acento no nome técnico; normalize espaços |
| `Revenda` | Nome do posto | Pode mudar ao longo do tempo; não use como chave |
| `CNPJ da Revenda` | **Identificador do posto** | Ler como texto; remover espaço; preservar a coluna original |
| `Nome da Rua`, `Numero Rua`, `Complemento`, `Bairro`, `Cep` | Endereço | Ler como texto, mesmo quando parece número |
| `Produto` | Combustível | Seis rótulos; `GASOLINA` ≠ `GASOLINA ADITIVADA` |
| `Data da Coleta` | Data da observação | Formato dia/mês/ano; teste com datas em que dia ≠ mês |
| `Valor de Venda` | Preço ao consumidor | Vírgula decimal; unidade depende do produto |
| `Valor de Compra` | Preço de distribuição | Vazio nesta edição |
| `Unidade de Medida` | Unidade do preço | Valide antes de comparar |
| `Bandeira` | Marca do posto | Inclui `BRANCA` (sem bandeira) |