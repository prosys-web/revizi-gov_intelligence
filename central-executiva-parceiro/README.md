# REVIZI — Central Executiva para Parceiro Financeiro (V0.4)

**Material demonstrativo | 27/11/2026 | ambiente separado do GOV Intelligence operacional**

## Abertura

Abra [index.html](./index.html) no navegador. A página inicial oferece quatro ambientes:

1. **Apresentação Comercial** — sete lâminas internas de narrativa comercial; duração proposta de até 10 minutos.
2. **Simulador Financeiro** — [simulador.html](./simulador.html), margens, capital, quantidade e valor de contratos, custos, tributos projetados e caixa.
3. **GOV Intelligence** — demonstração no `index.html` com recorte histórico de pregões do Ceará obtidos em 25/11/2026. Os registros não são dispensas nem atualização em tempo real.
4. **Mockup da Jornada Final** — [mockup.html](./mockup.html), com 24 oportunidades demonstrativas navegáveis, classificação por aderência e oito etapas: radar; edital/TR; itens e lotes; habilitação; fornecedores; precificação; robô de lances supervisionado; execução e recebimento.

## Escopo e limites

- **Demonstração de visão final**, não produto integrado ou homologado.
- O mockup não consulta PNCP, não se conecta a portais e **não envia lances**. Órgãos, fornecedores, requisitos, cotações, preços e resultados apresentados são simulados.
- A apresentação usa cenários financeiros hipotéticos de capital de R$ 100 mil, faturamento de R$ 400 mil e margens brutas de 20%, 30% e 40%. Não constituem retorno garantido, nem prova de margem média observada.
- O enquadramento no Simples Nacional e a tributação projetada são aproximações didáticas; exigem validação contábil.
- **60 dias** representam meta de desenvolvimento e homologação do fluxo integrado, condicionada a testes, fontes e permissões de integração de cada portal.
- O material é estático, sem bibliotecas externas, com arquivos HTML que funcionam localmente. Os links de navegação são relativos.
- O repositório e o painel operacional da REVIZI permanecem independentes desta demonstração.

## Segurança e governança

Não incluir credenciais, dados pessoais ou informações privadas de clientes neste diretório. Avaliar e auditar qualquer dependência ou código externo antes de sua incorporação. Preservar um aviso claro e único no início do mockup sobre a natureza simulada dos dados e funcionalidades em desenvolvimento.

## Arquivos

- `index.html` — Central Executiva e apresentação comercial
- `simulador.html` — simulador financeiro
- `mockup.html` — radar navegável com 24 processos, filtros, análise documental, itens e lotes, fornecedores, decisão, lances e execução
- `LEIA-ME.txt` — instruções de uso do pacote original

**Responsável pelo projeto:** REVIZI | GOV Intelligence.

## Referência de desenho

O radar reutiliza a lógica de tabela, filtros e aprofundamento do GOV Intelligence anterior e padrões de organização de painéis operacionais já utilizados em projetos reais. **Não utiliza dados privados ou transações da ARILUB**: todos os processos e números do mockup são gerados para demonstração.
