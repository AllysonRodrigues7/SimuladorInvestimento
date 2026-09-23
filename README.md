# 📊 Simulador de Investimentos em FIIs

Projeto desenvolvido durante um bootcamp da [DIO (Digital Innovation One)](https://www.dio.me/), com o objetivo de aplicar, na prática, fórmulas e recursos do Excel na criação de uma planilha de simulação de investimentos em Fundos de Investimento Imobiliário (FIIs).

## 📌 Sobre o projeto

A planilha permite ao usuário simular o crescimento de uma carteira de investimentos ao longo do tempo, a partir de um aporte mensal, e ainda sugerir uma distribuição de carteira entre diferentes tipos de FIIs, de acordo com o perfil de risco escolhido (Conservador, Moderado ou Agressivo).

## ⚙️ Funcionalidades

- **Configurações gerais**: definição de salário, rendimento médio da carteira e sugestão de valor de investimento mensal.
- **Simulador de investimento mensal**: cálculo do patrimônio acumulado e dos dividendos mensais estimados, a partir do valor investido, do prazo (em anos) e da taxa de rendimento mensal.
- **Cenários de longo prazo**: projeção automática do patrimônio e dos dividendos para 2, 5, 10, 20 e 30 anos.
- **Sugestão de carteira por perfil**: distribuição percentual sugerida entre os tipos de FII (Papel, Tijolo, Híbrido, FoF, Desenvolvimento e Hotelarias), calculada automaticamente conforme o perfil selecionado.

## 🧮 Fórmulas e recursos utilizados

- `FV` (Valor Futuro) — para projeção do patrimônio acumulado a partir de aportes mensais.
- `VLOOKUP` (PROCV) — para buscar o percentual sugerido de cada tipo de FII conforme o perfil de risco.
- Concatenação de texto (`&`) — para criar uma chave única (perfil + tipo de FII) usada na busca.
- Referências nomeadas (ex.: `taxa_mensal`, `aporte`, `rendimento_carteira`) — para deixar as fórmulas mais legíveis.
- `SUM` — para totalizar os valores distribuídos entre os tipos de FII.

## 🗂️ Estrutura da planilha

- **Planilha1**: tela principal, com as configurações, o simulador de investimento mensal, os cenários de longo prazo e a distribuição de carteira por perfil.
- **Planilha2**: tabela de apoio (base de dados), com os percentuais sugeridos para cada combinação de perfil de risco e tipo de FII.

## 🚀 Como usar

1. Abra o arquivo `Simulador_investimento.xlsx` no Excel ou em outro programa compatível (LibreOffice Calc, Google Sheets etc.).
2. Preencha os campos de entrada (em destaque) com o valor a investir por mês, o prazo em anos e a taxa de rendimento mensal esperada.
3. Escolha o perfil de risco desejado para ver a sugestão de distribuição entre os tipos de FII.
4. Confira os resultados: patrimônio acumulado, dividendos mensais e os cenários projetados.

## 🎯 Objetivo de aprendizado

Este projeto teve como foco praticar:
- Fórmulas financeiras no Excel (`FV`);
- Buscas de dados entre planilhas (`VLOOKUP`);
- Organização de dados e boas práticas de estruturação de planilhas;
- Lógica de simulação financeira aplicada a investimentos.

## 🛠️ Tecnologias

- Microsoft Excel (.xlsx)

---

Projeto feito para fins de estudo, como parte de um bootcamp da DIO.
