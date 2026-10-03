# simulador-finance-excel
Simulador de Investimentos em Fundos Imobiliários (FIIs)
Projeto desenvolvido como desafio prático do Bootcamp de Excel da DIO

Uma ferramenta interativa desenvolvida no Excel para auxiliar no planejamento financeiro focado em Fundos Imobiliários. Ela permite ao usuário simular a evolução do patrimônio ao longo do tempo e entender como distribuir seu aporte mensal de acordo com seu perfil de risco.

A ferramenta responde de forma direta e visual às cinco principais dúvidas do investidor:
1. Quanto investir por mês? -> Exibido no Painel de Entradas/Resumo (através da variável “aporte”).
2. Por quantos anos? -> Exibido no Resumo principal e detalhado na Tabela de Cenários (através da variável “anos”).
3. Qual a taxa de rendimento mensal? -> Definida na entrada de dados (através da variável “taxa_mensal”).
4. Quanto de patrimônio vai acumular? -> Calculado automaticamente via função “VF”.
5. Quanto vai receber de dividendos por mês? -> Calculado pela multiplicação do patrimônio acumulado pela taxa mensal de rendimento.

Lógica das Fórmulas Utilizadas
1. Função “VF” (Valor Futuro)
Utilizada para projetar o acúmulo de capital considerando aportes mensais constantes e juros compostos:
=VF(taxa_mensal; anos*12; -aporte)
