
# Histórias de Usuário – TaskFlow

## HU01 – Cadastro de usuário

**História:** Como visitante, quero criar uma conta no TaskFlow para poder acessar o sistema e organizar minhas tarefas.

**Prioridade:** Alta.

**Requisitos relacionados:** RF01, RNF01.

**Critérios de aceitação:**
1. O sistema deve permitir que o visitante informe os dados necessários para criar uma conta.
2. O sistema deve validar os dados informados.
3. Quando os dados forem válidos, o sistema deve criar a conta.
4. Após o cadastro, o usuário deve receber uma confirmação de que a conta foi criada.

## HU02 – Login

**História:** Como usuário cadastrado, quero realizar login para acessar minhas tarefas com segurança.

**Prioridade:** Alta.

**Requisitos relacionados:** RF02, RNF01, RNF03.

**Critérios de aceitação:**
1. O sistema deve permitir que o usuário informe suas credenciais.
2. O sistema deve permitir o acesso quando as credenciais forem válidas.
3. O sistema deve impedir o acesso quando as credenciais forem inválidas.
4. O usuário deve visualizar somente suas próprias tarefas.

## HU03 – Cadastrar tarefas

**História:** Como usuário cadastrado, quero cadastrar novas tarefas para organizar minhas atividades.

**Prioridade:** Alta.

**Requisitos relacionados:** RF03, RNF01, RNF02, RNF05.

**Critérios de aceitação:**
1. O sistema deve permitir o cadastro de uma nova tarefa.
2. O sistema deve validar os campos obrigatórios.
3. Após o cadastro, a tarefa deve aparecer na lista de tarefas do usuário.
4. Os dados da tarefa devem ser armazenados corretamente.

## HU04 – Editar tarefas

**História:** Como usuário cadastrado, quero editar minhas tarefas para atualizar suas informações.

**Prioridade:** Alta.

**Requisitos relacionados:** RF04, RNF01, RNF05.

**Critérios de aceitação:**
1. O sistema deve permitir selecionar uma tarefa existente.
2. O sistema deve permitir alterar as informações da tarefa.
3. O sistema deve salvar as alterações realizadas.
4. As informações atualizadas devem aparecer na lista de tarefas.

## HU05 – Excluir tarefas

**História:** Como usuário cadastrado, quero excluir tarefas para remover atividades que não preciso mais acompanhar.

**Prioridade:** Média.

**Requisitos relacionados:** RF05, RNF03, RNF05.

**Critérios de aceitação:**
1. O sistema deve permitir selecionar uma tarefa para exclusão.
2. O sistema deve solicitar confirmação antes de excluir.
3. Após a confirmação, a tarefa deve deixar de aparecer na lista.
4. O usuário não deve conseguir excluir tarefas pertencentes a outras contas.

## HU06 – Definir prioridades

**História:** Como usuário cadastrado, quero definir a prioridade das minhas tarefas para identificar quais atividades exigem mais atenção.

**Prioridade:** Alta.

**Requisitos relacionados:** RF06.

**Critérios de aceitação:**
1. O sistema deve oferecer as opções Alta, Média e Baixa.
2. O usuário deve conseguir selecionar uma prioridade para a tarefa.
3. A prioridade selecionada deve aparecer na tarefa.

## HU07 – Definir prazos

**História:** Como usuário cadastrado, quero definir prazos para minhas tarefas para acompanhar as datas de realização.

**Prioridade:** Alta.

**Requisitos relacionados:** RF07.

**Critérios de aceitação:**
1. O sistema deve permitir informar uma data para a tarefa.
2. O sistema deve armazenar o prazo informado.
3. O prazo deve aparecer nas informações da tarefa.

## HU08 – Atualizar status

**História:** Como usuário cadastrado, quero atualizar o status das minhas tarefas para acompanhar seu andamento.

**Prioridade:** Alta.

**Requisitos relacionados:** RF08.

**Critérios de aceitação:**
1. O sistema deve oferecer os status A fazer, Em andamento e Concluída.
2. O usuário deve conseguir alterar o status de uma tarefa.
3. O status atualizado deve aparecer na tarefa.

## HU09 – Consultar tarefas

**História:** Como usuário cadastrado, quero consultar minhas tarefas para acompanhar minhas atividades.

**Prioridade:** Alta.

**Requisitos relacionados:** RF09, RNF01, RNF02, RNF03.

**Critérios de aceitação:**
1. O sistema deve apresentar a lista de tarefas do usuário.
2. A consulta deve exibir as principais informações das tarefas.
3. O sistema deve apresentar os dados atualizados.
4. A consulta deve ser realizada em até 3 segundos.
5. O usuário deve visualizar somente suas próprias tarefas.

## HU10 – Pesquisar e filtrar tarefas

**História:** Como usuário cadastrado, quero pesquisar e filtrar minhas tarefas para encontrar atividades específicas com facilidade.

**Prioridade:** Média.

**Requisitos relacionados:** RF10, RNF01, RNF03.

**Critérios de aceitação:**
1. O sistema deve permitir pesquisar tarefas.
2. O sistema deve apresentar os resultados correspondentes à pesquisa.
3. O sistema deve permitir filtrar tarefas conforme os filtros disponíveis.
4. Quando não houver resultados, o sistema deve informar ao usuário.
5. A pesquisa e a filtragem devem considerar somente as tarefas do próprio usuário.
