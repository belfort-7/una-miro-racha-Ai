# RachaAí 💸

Protótipo de baixa fidelidade desenvolvido para a disciplina de **Interação Humano-Computador e UX** — Lista de Exercícios XV.  
Centro Universitário UNA · Professor Daniel Henrique Matos de Paiva

---

## 👤 Nome do Aluno / Equipe

Joao Victor Belfort Sousa Castro

---

## 🧩 Persona

**Estudantes universitários que dividem moradia.**

- **Nome:** Lucas, 22 anos
- **Perfil:** Mora em república com mais 3 colegas. Divide aluguel, conta de luz, internet e compras de mercado todo mês.
- **Dores:** Esquece de cobrar, tem vergonha de insistir, perde o controle de quem pagou o quê.
- **Necessidade:** Um app simples, rápido e transparente que faça as cobranças por ele — sem constrangimento.

---

## 🖼️ Telas do Protótipo

| # | Tela | Descrição |
|---|------|-----------|
| 1 | Dashboard de Grupos | Visão geral dos grupos ativos, saldo consolidado e alertas de cutucada |
| 2 | Detalhes do Grupo | Histórico de gastos do grupo com separação visual de débitos e créditos |
| 3 | Adicionar Gasto | Formulário com prévia da divisão antes de confirmar |
| 4 | Câmera / Scanner de NF | Interface de leitura de nota fiscal com extração automática de valores |
| 5 | Extrato de Dívidas | Visão clara de quem deve para quem, com botão de Pagar e Cutucar |
| 6 | Confirmação de Pagamento | Feedback visual de transação liquidada com barra de progresso |

> Arquivos disponíveis em `/prototipo/`

---

## 🎯 Heurística de Nielsen em Foco

### ****#1 — Visibilidade do Status do Sistema****

O RachaAí foi projetado para que o usuário **nunca fique no escuro** sobre o que está acontecendo:

- Na tela de **câmera**, os itens extraídos da nota fiscal aparecem em tempo real, antes de qualquer confirmação.
- Na tela de **adicionar gasto**, a prévia da divisão é exibida instantaneamente conforme o usuário seleciona participantes e método.
- Na tela de **confirmação**, a barra de progresso preta completa reforça visualmente que a dívida foi zerada.
- No **dashboard**, o saldo negativo aparece em destaque no topo — o usuário sabe imediatamente o que está devendo ao abrir o app.

> *"O sistema deve sempre manter os usuários informados sobre o que está acontecendo, por meio de feedback adequado dentro de um tempo razoável."* — Jakob Nielsen

---

## 🗺️ Fluxo de Tarefa

### Cadastrar uma conta de luz e dividir entre 3 pessoas

```
1. Abrir o app → Dashboard exibe os grupos ativos

2. Tocar no grupo "Casa"
   → Abre a tela de Detalhes do Grupo

3. Tocar em "+ Adicionar gasto"
   → Abre o formulário de Novo Gasto

4. Preencher o valor: R$ 130,00

5. Preencher a descrição: "Conta de luz"
   → Selecionar categoria: Contas

6. Definir quem pagou: tocar em "Trocar" e selecionar Ana

7. Selecionar os participantes: marcar Ana, Pedro e Rafa (3 pessoas)
   → Desmarcar Lucas se necessário

8. Escolher o método de divisão: "Igual"
   → Prévia exibe R$ 43,33 para cada um

9. Tocar em "Confirmar gasto"
   → Gasto registrado; grupo atualizado

10. Ana recebe notificação de que o gasto foi adicionado
    Pedro e Rafa recebem alerta de débito pendente
```

---

## ⭐ Desafio Extra (Opcional)

### Fluxo de Disputa — Valor cadastrado errado

```
1. Na tela de Detalhes do Grupo, tocar no gasto incorreto

2. Tocar no menu "···" (opções) no canto superior direito

3. Selecionar "Contestar gasto"

4. Inserir o valor correto e uma justificativa (ex: "NF mostra R$ 110,00")

5. O sistema notifica quem cadastrou o gasto original
   → Ele pode aceitar a correção ou rejeitar

6. Se aceito: gasto atualizado, divisão recalculada automaticamente
   Se rejeitado: disputa fica marcada como "em aberto" para resolução manual
```

### Relatório Mensal

Uma tela de **Relatório Mensal** mostra em que a casa mais gastou, com um gráfico de barras simples:

```
Mercado       ████████████  R$ 480,00
Contas fixas  ████████      R$ 310,00
Lazer         ████          R$ 160,00
Transporte    ██            R$ 80,00
```

Acessível pelo perfil do grupo → "Ver relatório".

---

## 🛠️ Ferramenta Utilizada

- **Miro** — prototipagem de baixa fidelidade
- Exportado em `.png` e `.pdf`

---

## 📁 Estrutura do Repositório

```
ihcux-racha-ai/
├── prototipo/
│   ├── tela1_dashboard.png
│   ├── tela2_detalhes_grupo.png
│   ├── tela3_adicionar_gasto.png
│   ├── tela4_camera_nf.png
│   ├── tela5_extrato_dividas.png
│   ├── tela6_confirmacao.png
│   └── prototipo.pdf
└── README.md
```

---

## 💡 Insight de IHC

> *Lidar com dinheiro gera ansiedade.* O RachaAí transmite segurança através da transparência: cada ação tem uma confirmação clara, cada valor tem uma prévia antes de ser efetivado, e o sistema assume a parte "chata" das cobranças com o mecanismo de Cutucada — preservando os relacionamentos entre os moradores.
