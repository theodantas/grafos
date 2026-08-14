<h1 align="center">Rede de Entrosamento da Seleção Brasileira ⚽📊</h1>

<p align="center"><i>Da Modularidade Regional ao Mundo Pequeno Globalizado (1958–2026)</i></p>

![Preview do dashboard interativo](preview.gif)

<h4 align="center"><a href="https://theodantas.github.io/grafos/">Confira o projeto aqui</a></h4>

---

## 📌 Sobre o Projeto

Este projeto foi desenvolvido para a disciplina **BC-0506: Comunicação e Redes**, da **Universidade Federal do ABC (UFABC)**, ministrada pelo Prof. João Henrique Kleinschmidt.

O objetivo é modelar e analisar, sob a ótica da **Teoria de Redes Complexas**, a evolução do entrosamento entre os jogadores convocados para a Seleção Brasileira de Futebol em cinco recortes temporais: **1958, 1970, 1994, 2002 e uma projeção para 2026**.

A hipótese investigada é que a rede de entrosamento evoluiu de uma estrutura **modular**, organizada em torno de clubes brasileiros tradicionais (Santos, Botafogo, Vasco), para uma estrutura de **Mundo Pequeno globalizado**, sustentada por hubs internacionais (Real Madrid, Arsenal, PSG). Essa transição reflete, em termos de rede, o processo histórico de internacionalização das carreiras dos jogadores brasileiros.

## 🧠 Modelagem

- **Vértices:** jogadores convocados em cada edição da Seleção
- **Arestas:** clube profissional compartilhado entre dois jogadores (entrosamento prévio)
- **Peso da aresta:** número de clubes em comum entre o par de jogadores
- **Grafo:** não-direcionado e ponderado, um para cada convocação analisada

## 📈 Métricas e Conceitos Aplicados

✔️ Centralidade de Grau (jogadores mais "conectados" de cada elenco);
✔️ Modularidade (algoritmo de Louvain) — identificação de comunidades/clãs de clubes;
✔️ Diâmetro da rede e densidade;
✔️ Coeficiente de agrupamento (clustering);
✔️ Conceito de Redes de Mundo Pequeno (*Small World*, Watts & Strogatz);
✔️ Identificação de "clubes-ponte" entre comunidades;
✔️ Visualização de grafos com layout de força (ForceAtlas2 / D3 force simulation).

## 🔎 Principais Achados

| Ano | Modularidade | Diâmetro | Padrão observado |
|---|---|---|---|
| 1958 | Alta (0,66) | 3 | Comunidades fechadas por clube nacional |
| 1970 | Alta (0,62) | 3 | Persistência dos clãs regionais |
| 1994 | Baixa (0,25) | 3 | Início da integração com o futebol europeu |
| 2002 | Baixa (0,30) | 3 | Rede mais densa do conjunto analisado |
| 2026 | Moderada (0,36) | 5 | Rede globalizada, porém mais dispersa geograficamente |

O resultado mais interessante do projeto foi justamente **contrariar a hipótese inicial**: o diâmetro de 2026 é maior que o de 1994/2002, não menor — mostrando que a globalização ampliou a diversidade de clubes sem necessariamente aumentar a coesão direta entre os jogadores.

## 🛠 Tecnologias Utilizadas

<div>
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
    <img src="https://img.shields.io/badge/NetworkX-2E9B6B?style=for-the-badge&logo=graph&logoColor=white" />
    <img src="https://img.shields.io/badge/D3.js-F9A03C?style=for-the-badge&logo=d3.js&logoColor=white" />
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
</div>

- **Python (Pandas, NetworkX, python-louvain):** tratamento dos dados e cálculo das métricas de rede
- **D3.js:** simulação de forças (force-directed graph) para a visualização interativa
- **Gephi:** layout ForceAtlas2 usado na apresentação em slides
- **ReportLab:** geração das tabelas comparativas no PDF complementar

## 🎓 Disciplina e Contexto Acadêmico

**Disciplina:** BC-0506 — Comunicação e Redes
**Instituição:** Universidade Federal do ABC (UFABC)
**Professor:** João Henrique Kleinschmidt
**Período:** 2026

---

<table align="center">
  <tr>
    <td>
      <img src="https://github.com/theodantas.png" width="100px"/>
    </td>
    <td>
      Feito por <a href="https://github.com/theodantas">Théo Dantas.</a> 🙋‍♂️
    </td>
  </tr>
</table>
