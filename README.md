# mascara_dashboard

Skill para o Claude que transforma sites, landing pages e dashboards com "cara de feito por IA" em interfaces com acabamento de designer profissional, em português e com padrões brasileiros (R$, datas, textos sem hype).

## O que ela faz

1. Audita os sinais de interface gerada por IA: gradiente roxo, glow, emoji nos rótulos, texto com gradiente, "Bem-vindo de volta! 👋", CAIXA ALTA espaçada etc.
2. Define uma direção a partir do próprio produto (personalidade, mundo, momentos de destaque, assinatura)
3. Mostra a auditoria e a direção e espera aprovação
4. Corrige em 9 passadas: espaçamento, cor, ícones, texto, tipografia, layout, detalhes, visuais e animação
5. Confere com um checklist, incluindo o "teste do template"

Funciona com HTML, CSS, Tailwind e React, a partir de código, de um link ou de um print.

## Instalação

- **Claude.ai:** baixe `skills/mascara-dashboard` como .zip e envie em Configurações → Capacidades → Skills
- **Claude Code:** copie a pasta `skills/mascara-dashboard` para `~/.claude/skills/`

Depois é só pedir: "deixa esse dashboard com cara de profissional".

## Crédito e licença

Adaptação em português do [unslop](https://github.com/heydamir/unslop), de Damir Sokolovsky ([@heydamir](https://x.com/heydamir)). Licença [CC BY 4.0](LICENSE) — mantenha o crédito em cópias e adaptações.
