
# Requisitos Funcionais – TaskFlow

## Introdução

Este documento apresenta os requisitos funcionais do TaskFlow, um sistema de gerenciamento de tarefas que permite aos usuários cadastrados organizar, acompanhar, consultar e atualizar suas atividades.

## Requisitos

### RF01 – Cadastro de usuários
- **Descrição:** O sistema deverá permitir que visitantes criem uma conta, informando os dados necessários para o cadastro.
- **Processamento:** O sistema deverá validar os dados informados e realizar o cadastro quando forem válidos.
- **Saída:** O sistema deverá informar se a conta foi criada ou se ocorreu algum erro.
- **Prioridade:** Alta

### RF02 – Login
- **Descrição:** O sistema deverá permitir que usuários cadastrados acessem suas contas por meio de suas credenciais.
- **Processamento:** O sistema deverá verificar as credenciais informadas.
- **Saída:** O sistema deverá permitir o acesso quando forem válidas e informar quando forem inválidas.
- **Prioridade:** Alta

### RF03 – Cadastrar tarefas
- **Descrição:** O sistema deverá permitir que usuários cadastrados criem novas tarefas.
- **Entrada:** Título, descrição, prazo, prioridade e status da tarefa.
- **Processamento:** O sistema deverá registrar as informações da tarefa e associá-la ao usuário responsável.
- **Saída:** O sistema deverá informar o resultado do cadastro e apresentar a tarefa registrada.
- **Prioridade:** Alta

### RF04 – Editar tarefas
- **Descrição:** O sistema deverá permitir que usuários cadastrados alterem as informações de suas tarefas existentes.
- **Entrada:** Tarefa selecionada e novas informações de título, descrição, prazo, prioridade ou status.
- **Processamento:** O sistema deverá atualizar os dados da tarefa selecionada.
- **Saída:** O sistema deverá apresentar as informações atualizadas.
- **Prioridade:** Alta

### RF05 – Excluir tarefas
- **Descrição:** O sistema deverá permitir que usuários cadastrados excluam suas próprias tarefas.
- **Entrada:** Tarefa selecionada para exclusão e confirmação da operação.
- **Processamento:** O sistema deverá excluir a tarefa após a confirmação.
- **Saída:** A tarefa excluída não deverá aparecer nas consultas posteriores.
- **Prioridade:** Média

### RF06 – Definir prioridades
- **Descrição:** O sistema deverá permitir que o usuário defina a prioridade de cada tarefa.
- **Entrada:** Uma das opções: Alta, Média ou Baixa.
- **Processamento:** O sistema deverá registrar a prioridade selecionada na tarefa.
- **Saída:** A prioridade deverá aparecer nas informações da tarefa.
- **Prioridade:** Alta

### RF07 – Definir prazos
- **Descrição:** O sistema deverá permitir que o usuário informe ou altere o prazo de uma tarefa.
- **Entrada:** Data selecionada para a tarefa.
- **Processamento:** O sistema deverá registrar o prazo informado.
- **Saída:** O prazo deverá aparecer nas informações da tarefa.
- **Prioridade:** Alta

### RF08 – Atualizar status
- **Descrição:** O sistema deverá permitir que o usuário atualize o andamento de suas tarefas.
- **Entrada:** Um dos status disponíveis: A fazer, Em andamento ou Concluída.
- **Processamento:** O sistema deverá atualizar o status da tarefa selecionada.
- **Saída:** O sistema deverá apresentar o novo status.
- **Prioridade:** Alta

### RF09 – Consultar tarefas
- **Descrição:** O sistema deverá permitir que usuários cadastrados visualizem suas tarefas.
- **Entrada:** Solicitação de consulta das tarefas.
- **Processamento:** O sistema deverá buscar as tarefas associadas à conta do usuário.
- **Saída:** O sistema deverá apresentar a lista de tarefas com suas informações atualizadas.
- **Prioridade:** Alta

### RF10 – Pesquisar e filtrar tarefas
- **Descrição:** O sistema deverá permitir que usuários cadastrados pesquisem e filtrem suas tarefas.
- **Entrada:** Termo de pesquisa ou critérios de filtragem disponíveis no sistema.
- **Processamento:** O sistema deverá localizar as tarefas que correspondam aos critérios informados, considerando somente as tarefas do usuário.
- **Saída:** O sistema deverá apresentar os resultados encontrados ou informar quando não houver resultados.
- **Prioridade:** Média

## Regras gerais

- Cada usuário deverá ter acesso somente às suas próprias tarefas.
- As prioridades disponíveis serão Alta, Média e Baixa.
- Os status disponíveis serão A fazer, Em andamento e Concluída.
- As alterações realizadas nas tarefas deverão ser refletidas nas consultas posteriores.
