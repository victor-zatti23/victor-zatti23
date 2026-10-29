# Victor Zatti

**Português** · [English](README.en.md)

**QA que automatiza QA com IA.** Testo plataformas de investimento (web, API e mobile) e construo as ferramentas que decidem *o que* testar, *como* provar que passou e *onde* registrar a evidência.

Hoje o código é escrito cada vez mais por IA e chega rápido demais para revisar na mão. Meu trabalho é fazer o teste acompanhar esse ritmo sem perder o critério de aceite de vista.

---

### O que eu faço

- **QA orientado a risco**: leio o que mergeou no dia e ordeno pelo que pode quebrar produção, não pela ordem de chegada.
- **Automação web e de API**: Playwright com login real (Keycloak), sessão salva e conferência pela API em vez de confiar só na tela.
- **Mobile**: roteiros no simulador iOS e em Android físico com Maestro, prints de cada passo como evidência.
- **Agentes de IA no fluxo**: skills de Claude Code que transformam bug descrito em português em card estruturado, executam roteiros e fecham o laudo em PDF.
- **Multiagente para desenvolvimento**: orquestrador + dev back + dev front + revisor, com QA isolado como portão de saída.

### Projetos

| Projeto | O que resolve |
|---|---|
| [qa-risk-queue](https://github.com/victor-zatti23/qa-risk-queue) | Numa esteira que foi de 19 para 803 PRs/mês, com a maioria mergeada sem approval, responde todo dia: *o que eu testo hoje?* Score por natureza da mudança (prod, autorização, contrato, config), agrupado por card. |
| playwright-qa-harness _(em breve)_ | Harness de QA web: login, provisionamento de conta de teste, oráculo pela API e relatório HTML com prints. |
| mobile-qa-maestro _(em breve)_ | Flows de Maestro para iOS e Android, rodando em simulador e device real. |
| claude-qa-skills _(em breve)_ | Skills de Claude Code para QA: bug → card estruturado, plano de teste, relatório diário em PDF. |
| multi-agent-dev-flow _(em breve)_ | Como montei um time de agentes (Opus + Sonnet) para implementar cards, com custo real, o que o revisor pegou e os portões que impedem CI vermelho. |

### Ferramentas

`Playwright` · `Maestro` · `Cypress` · `Postman` · `SQL` · `Node.js` · `GitHub API (GraphQL)` · `Jira` · `Azure DevOps` · `Claude Code` · `Agentes de IA / MCP`

### Como eu penso teste

- Tela não é oráculo. Se a API ou o banco disser outra coisa, a tela está mentindo.
- Todo caso tem evidência: print do passo, não "testei e passou".
- Teste unitário a IA já escreve. O buraco está no critério de aceite, na integração entre telas e na paridade de configuração entre ambientes.

