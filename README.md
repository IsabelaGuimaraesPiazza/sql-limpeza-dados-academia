# Desafio SQL: Cruzamento e Higienização de Dados de Acessos

Projeto prático desenvolvido em SQL para simular o tratamento e a consolidação de dados brutos vindos de um sistema de catracas de uma academia.

## Cenário do Problema
O banco de dados recebia registros de alunos com problemas de formatação (espaços em branco em excesso e letras em formatos mistos) e inconsistências em campos cruciais, como planos de assinatura não preenchidos (`NULL`). O objetivo foi cruzar o histórico de acessos diários com o cadastro desses alunos, entregando um relatório limpo e padronizado para a equipe de negócios.

## Tecnologias e Conceitos Aplicados
- **INNER JOIN**: Cruzamento de tabelas (`frequencia` e `alunos`) utilizando chaves primárias e estrangeiras.
- **Funções de String (`TRIM` e `UPPER`)**: Remoção de espaçamentos inúteis nas pontas e padronização dos nomes dos clientes em caixa alta.
- **Tratamento de Valores Nulos (`COALESCE`)**: Substituição de campos vazios (`NULL`) pelo texto padrão `'Sem plano'`, evitando falhas em relatórios visuais.
- **Aliases (Apelidos de Tabelas)**: Uso de boas práticas de legibilidade e identificação de origem de colunas.

## 📊 Estrutura do Script
O repositório contém o script estruturado contendo:
1. O **Schema** para criação das tabelas.
2. Os **Dados de Teste** (massa de dados bruta).
3. A **Query Final** de tratamento e consulta.
