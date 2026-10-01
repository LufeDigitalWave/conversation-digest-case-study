# Consolidação periódica de conversas

Case técnico anonimizado sobre organização de mensagens e geração periódica de resumos.

> Publicação documental. Não contém conversas, participantes, identificadores de grupos, modelos de prompt privados ou integrações ativas.

## Problema

Um resumo periódico precisa considerar a janela correta de mensagens, evitar processamento duplicado e distinguir o que foi discutido do que efetivamente foi decidido. Uma falha no processamento não pode descartar silenciosamente o histórico pendente.

## Escopo representado

Separação entre obtenção de mensagens, persistência, tarefas de coleta e consolidação, serviço de geração e controle de configuração. Esses componentes foram identificados na estrutura de origem, sem copiar mensagens ou contratos de provedores.

## Stack identificada

TypeScript, Prisma e Zod. O projeto de origem contém tarefas separadas de coleta e resumo; esta publicação não executa essas tarefas nem um modelo de linguagem.

## O que discutir numa entrevista

- Como definir uma janela sem omitir nem repetir mensagens.
- Como lidar com mensagens atrasadas e execuções interrompidas.
- Como distinguir síntese, citação e atribuição de decisão.
- Como limitar retenção e acesso ao conteúdo processado.

Consulte a [arquitetura e o roteiro de validação](ARCHITECTURE.md).

## Limites

Não são publicadas conversas reais ou exemplos derivados delas. Não há alegação de precisão dos resumos, execução automática confiável ou suíte de testes aprovada.
