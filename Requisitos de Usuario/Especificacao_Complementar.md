
# Especificação Complementar – TaskFlow

## 1. Introdução

Este documento complementa os requisitos funcionais, não funcionais e as histórias de usuário do TaskFlow, detalhando premissas, restrições, ambiente de execução, entradas, saídas e situações de erro do sistema.

## 2. Premissas

- O usuário deverá possuir uma conta para acessar e gerenciar suas tarefas.
- O usuário deverá informar dados válidos para realizar operações no sistema.
- O sistema deverá estar disponível para uso quando os serviços necessários estiverem funcionando.
- Cada tarefa deverá estar associada ao usuário que a cadastrou.

## 3. Restrições

- Somente usuários cadastrados e autenticados poderão gerenciar tarefas.
- Cada usuário poderá consultar e modificar somente suas próprias tarefas.
- As prioridades disponíveis serão Alta, Média e Baixa.
- Os status disponíveis serão A fazer, Em andamento e Concluída.
- O desempenho de cadastro e consulta deverá respeitar o limite de até 3 segundos em condições normais de uso.
- O sistema deverá funcionar nos navegadores Google Chrome, Mozilla Firefox e Microsoft Edge.

## 4. Ambiente de execução

### 4.1 Software
- Sistema operacional: ambiente compatível com a aplicação.
- Navegadores: Google Chrome, Mozilla Firefox e Microsoft Edge.
- Banco de dados: serviço de armazenamento utilizado pela aplicação.
- Aplicação: sistema TaskFlow executado em ambiente compatível com sua implementação.

### 4.2 Hardware
O sistema deverá funcionar em computadores capazes de executar o sistema operacional, o navegador e os serviços necessários para a aplicação.

Não foi definido um requisito mínimo específico de processador, memória RAM ou armazenamento.

## 5. Entradas, processamento e saídas

| Funcionalidade | Entrada | Processamento | Saída |
|---|---|---|---|
| Cadastro | Dados do usuário | Validar e cadastrar | Confirmação ou mensagem de erro |
| Login | Credenciais | Verificar credenciais | Acesso ou mensagem de erro |
| Cadastro de tarefa | Título, descrição, prazo, prioridade e status | Validar e armazenar tarefa | Confirmação e tarefa cadastrada |
| Edição | Tarefa selecionada e novos dados | Atualizar informações | Tarefa atualizada |
| Exclusão | Tarefa selecionada e confirmação | Excluir tarefa | Confirmação da exclusão |
| Prioridade | Alta, Média ou Baixa | Atualizar prioridade | Prioridade atualizada |
| Prazo | Data informada | Armazenar prazo | Prazo atualizado |
| Status | A fazer, Em andamento ou Concluída | Atualizar status | Status atualizado |
| Consulta | Solicitação de consulta | Buscar tarefas do usuário | Lista de tarefas |
| Pesquisa e filtragem | Termo ou critérios disponíveis | Localizar tarefas correspondentes | Resultados ou aviso de ausência de resultados |

## 6. Tratamento de situações de erro

- **Dados inválidos no cadastro:** o sistema deverá informar que os dados precisam ser corrigidos.
- **Credenciais incorretas:** o sistema deverá impedir o login e apresentar uma mensagem de erro.
- **Campos obrigatórios vazios:** o sistema deverá solicitar o preenchimento dos campos necessários.
- **Tarefa inexistente:** o sistema deverá informar que a tarefa não foi encontrada.
- **Acesso não autorizado:** o sistema deverá impedir o acesso a tarefas pertencentes a outros usuários.
- **Falha no armazenamento:** o sistema deverá informar que não foi possível concluir a operação.
- **Pesquisa sem resultados:** o sistema deverá informar que nenhuma tarefa foi encontrada.

## 7. Estados do sistema

### 7.1 Estado inicial
Ao acessar o sistema, o visitante deverá visualizar a opção de cadastro ou login.

### 7.2 Usuário não autenticado
O visitante poderá realizar o cadastro ou tentar acessar uma conta existente, mas não poderá gerenciar tarefas.

### 7.3 Usuário autenticado
Após realizar o login com sucesso, o usuário poderá acessar e gerenciar suas próprias tarefas.

### 7.4 Operação em andamento
Durante o cadastro, edição ou exclusão, o sistema deverá processar a solicitação e apresentar o resultado da operação.

### 7.5 Encerramento da sessão
Quando o usuário sair do sistema, deverá deixar de ter acesso às funcionalidades restritas até realizar um novo login.

### 7.6 Falha durante uma operação
Se ocorrer uma falha, o sistema deverá informar que a operação não foi concluída e preservar os dados já armazenados corretamente.

## 8. Tipos de dados e limites

| Informação | Tipo de dado | Regra |
|---|---|---|
| Título da tarefa | Texto | Campo obrigatório |
| Descrição | Texto | Campo descritivo |
| Prazo | Data | Data informada pelo usuário |
| Prioridade | Opção enumerada | Alta, Média ou Baixa |
| Status | Opção enumerada | A fazer, Em andamento ou Concluída |
| Dados de cadastro | Texto | Devem ser validados |
| Credenciais | Texto | Devem ser verificadas no login |

Os limites máximos de caracteres, tamanho dos campos e quantidade de tarefas por usuário ainda não foram definidos.

## 9. Interfaces e comunicação

- **Interface com o usuário:** deverá permitir cadastro, login e gerenciamento de tarefas.
- **Interface com o banco de dados:** deverá permitir armazenar, consultar, atualizar e excluir informações.
- **Interface com o navegador:** deverá permitir a utilização do sistema nos navegadores especificados.
- **Interface de mensagens:** deverá apresentar confirmações, resultados e avisos de erro das operações.

## 10. Fluxo de informações

1. O visitante informa seus dados para criar uma conta.
2. O sistema valida e registra o cadastro.
3. O usuário informa suas credenciais para realizar login.
4. O sistema verifica o acesso e identifica a conta.
5. O usuário cadastra, consulta, edita, pesquisa, filtra ou exclui suas tarefas.
6. O sistema processa as operações e atualiza os dados armazenados.
7. As informações atualizadas são apresentadas ao usuário.

## 11. Considerações finais

Esta especificação complementar detalha aspectos necessários para melhorar a compreensão, implementação e validação do TaskFlow. Os pontos ainda não definidos, como limites máximos dos campos e requisitos mínimos de hardware, deverão ser estabelecidos conforme as decisões de implementação do projeto.
