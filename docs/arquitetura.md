# Arquitetura conceitual — GOV Intelligence

Status: proposta, sujeita a validação técnica e comercial.

## Fluxo
Fontes públicas autorizadas → aquisição → normalização → evidências → motores de inteligência → workflow → revisão humana → aprendizado.

| Camada | Responsabilidade |
|---|---|
| Conectores | PNCP, Compras.gov e fontes regionais após validação de acesso e cobertura |
| Dados | Identificadores, procedência, datas, deduplicação, unidades, versão e qualidade |
| Inteligência | Radar, Edital IA, mercado, preços, competição, risco e score |
| Operação | Pipeline, alertas, tarefas, integrações e aprovações |
| Segurança | Autenticação, isolamento por cliente, mínimo privilégio, segredos no backend |
| Observabilidade | Logs sanitizados, métricas, idempotência, timeout, retentativa e rollback |

## Contratos de dados
Cada evidência deve registrar fonte, identificador, data de coleta, período, cobertura e nível de confiança. Ausência de evidência não equivale a risco baixo. Preços exigem comparação de unidade, quantidade, especificação, região e período. Diferenciar valores estimados, propostas e homologados. Separar modalidade de contratação de sistema de registro de preços.

## Módulos
1. Radar: filtros por perfil e categoria, deduplicação e alertas.
2. Edital IA: extração com referência à página/trecho, sinalização de dúvida e revisão humana.
3. Mercado: tendências por categoria, órgão, região e período.
4. Preços: distribuição histórica e comparáveis, sem prometer preço vencedor.
5. Competição: resultados e atas públicas; sequência de lances apenas quando disponível.
6. Recebimento: empenho, liquidação e pagamento quando relacionáveis; mediana, P75, P90, tamanho da amostra.
7. Risco: comercial, financeiro, fornecedor, execução e documentação; bloqueios explícitos e revisão humana.
8. Decisão: aprovar, revisar, não participar, com justificativa e histórico.

## Pipeline
Identificada → análise → apta → aprovação → proposta → disputa → resultado → homologação/contratação → execução → recebimento. Registrar saídas laterais, suspensão e revogação. Adaptar aos eventos reais de cada procedimento.

## Limites
Nenhum conector ou motor é declarado operacional por este documento. Não executar lances automaticamente. Validar disponibilidade e termos das fontes. Dados reais e implementação proprietária ficam em ambiente privado e autorizado.
