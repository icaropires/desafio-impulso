# Desafio Impulso

Repositório que contém minha resposta ao desafio proposto pela impulsoGov para a vaga de estagiário em ciência de dados

## Desafio Modelagem & Análise 📊

#### 1. Como comparar municípios? (descritiva)

Imagine que um gestor público entra hoje no Farol e quer ter a possibilidade de comparar seu município com outros municípios de seu interesse.

**(a) Como você selecionaria municípios para comparação? Descreva quais caracaterísticas você selecionaria para definir municípios semelhantes.**

Sobre a equivalência entre municípios, dificilmente se elaboraria um método com 100% de eficácia, mas acredito que uma boa aproximação seria entre municípios:

* Da mesma região do Brasil (Norte, Nordeste, etc.)
* Políticas públicas parecidas
* Clima parecido
* Número de habitantes parecidos
* Verba do governo semelhante
* Distribuição das atividades econômicas semelhante (uma cidade não pode ser focada em mineração e outra em pecuária)
* Distribuição dos moradores entre área rural e urbana semelhante
* Distribuição de renda semelhante

com isso, consequentemente o IDH muito provavelmente será também parecido e os municípios comparáveis.

**(b) Descreva 2 (duas) análises ou visualizações que você montaria para comparar a situação entre esses municípios.**

1. **Recursos disponíveis.**
Indicadores:
* Número de leitos/respiradores disponíveis
* Número de leitos/respiradores total
* Número de testes disponíveis
* Quantidade de testes já realizados
* Dinheiro já investido no combate ao vírus (incluindo públicas, ajuda humanitária, etc.)
* Nível de desemprego

Aqui boa parte dos tipos de gráficos não atenderia, por estarmos tratando de valores com escalas muito diferentes entre sí.
Provavelmente uma dashboard com textos, com valores absolutos, mas com fontes de tamanhos variados, cores e ícones já atenderia ao objetivo.

2. Pessoas infectadas
Indicadores:
* Quantidade da população que já pegou o vírus
* Quantidade de pessoas que veio a falecer
* Quando aconteceu (ou está previsto) o pico da doença

Aqui, um simples gráfico em barras, normalizando os valores pela porcentagem da população, já atenderia aos primeiros dois
tópicos. Sobre a data do pico, o ideal seria um gráfico em linha, em que o aumento ou diminuição da taxa de casos fique
bem visível, e, por consequência, os pontos críticos da curva.


#### 2. Como você montaria um dashboard para a gestão municipal? (Jupyter notebook)

Disponível no jupyter `30-08 Desafio Análise de Dados.ipynb`
