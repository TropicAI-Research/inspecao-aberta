# Inspeção Aberta

Prova de conceito (POC) com os dados públicos de condenação da inspeção federal (PGA-SIGSIF/MAPA) para suínos, organizados em um mapa interativo e em gráficos de barras.

**Acesse a página:** https://tropicai-research.github.io/inspecao-aberta/

## O que a página mostra

- **Mapa:** estabelecimentos com SIF que abatem suínos, posicionados pelo endereço do CNPJ na Receita Federal. O tamanho e a cor de cada ponto indicam a quantidade desviada no filtro atual. Clicando em um ponto, abre o detalhamento do estabelecimento.
- **Barras:** ocorrências por mês empilhadas por destino (condenado, reaproveitado, liberado e outros), os principais diagnósticos e os estados com mais ocorrências.
- **Filtros:** região, UF, busca por nome ou município, período, parte do animal, diagnóstico e destinos. Os filtros valem para o mapa, para as barras e para o relatório que pode ser baixado ou impresso.

Os dados cobrem de janeiro de 2024 a julho de 2026. Julho de 2026 está incompleto, porque a coleta foi feita no meio do mês.

## Cuidados na leitura

- A quantidade se refere a partes ou carcaças afetadas lançadas no sistema. Uma mesma carcaça com mais de um diagnóstico pode ser contada mais de uma vez.
- A coluna "UF" do SIGSIF não foi usada para posicionar os pontos, porque a documentação oficial não deixa claro se ela indica o estado do estabelecimento ou a procedência dos animais.
- Foram retirados 65 registros com diagnósticos incompatíveis com a espécie, como doenças de aves, equinos, ovinos e pescado lançadas em suínos.

## Fontes de dados

- [PGA-SIGSIF: consulta pública de Condenação de Animais por Espécie](https://sistemas.agricultura.gov.br/pga_sigsif/pages/view/sigsif/condenacaoanimal/index.xhtml)
- [PGA-SIGSIF: consulta pública de Abate por Sexo e UF](https://sistemas.agricultura.gov.br/pga_sigsif/pages/view/sigsif/abatesexouf/indexAbateSexoPorUf.xhtml)
- [Portal de Dados Abertos do MAPA: conjunto PGA-SIGSIF](https://dados.agricultura.gov.br/dataset/servico-de-inspecao-federal-sif) (CSVs de condenação, abates, estabelecimentos e dicionários de dados)
- [IBGE/SIDRA: Pesquisa Trimestral do Abate de Animais, tabela 1093](https://sidra.ibge.gov.br/tabela/1093)
- Receita Federal (dados cadastrais públicos de CNPJ), usada para localizar os estabelecimentos

## Licença

MIT. Os dados são públicos e pertencem às respectivas fontes.
