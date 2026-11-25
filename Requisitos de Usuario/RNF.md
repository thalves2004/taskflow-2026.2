
# Requisitos Não Funcionais – TaskFlow

## Introdução

Este documento apresenta os requisitos não funcionais do TaskFlow, definindo critérios de qualidade, segurança, desempenho, usabilidade, compatibilidade e confiabilidade do sistema.

## Requisitos

### RNF01 – Usabilidade
- **Descrição:** O sistema deverá apresentar uma interface simples e intuitiva, permitindo que os usuários encontrem e utilizem as principais funcionalidades sem dificuldades.
- **Categoria:** Usabilidade
- **Prioridade:** Alta
- **Critério de verificação:** Verificar se um usuário consegue cadastrar, editar, excluir e consultar uma tarefa sem precisar de instruções externas.
- **Relacionado a:** RF03, RF04, RF05 e RF09.

### RNF02 – Desempenho
- **Descrição:** O sistema deverá responder às operações de cadastro e consulta de tarefas em até 3 segundos, considerando condições normais de uso.
- **Categoria:** Desempenho
- **Prioridade:** Alta
- **Critério de verificação:** Medir o tempo entre a solicitação e a apresentação do resultado das operações de cadastro e consulta. O tempo deverá ser de até 3 segundos.
- **Relacionado a:** RF03 e RF09.

### RNF03 – Segurança
- **Descrição:** O sistema deverá proteger as informações dos usuários, garantindo que cada usuário autenticado possa acessar e modificar somente suas próprias tarefas.
- **Categoria:** Segurança
- **Prioridade:** Alta
- **Critério de verificação:** Realizar testes com contas diferentes e verificar se um usuário não consegue consultar, editar ou excluir tarefas pertencentes a outro usuário.
- **Relacionado a:** RF01, RF02, RF03, RF04, RF05, RF06, RF07, RF08, RF09 e RF10.

### RNF04 – Compatibilidade
- **Descrição:** O sistema deverá funcionar nos navegadores modernos Google Chrome, Mozilla Firefox e Microsoft Edge.
- **Categoria:** Compatibilidade
- **Prioridade:** Média
- **Critério de verificação:** Testar as principais funcionalidades do sistema nos três navegadores indicados, verificando se apresentam funcionamento adequado.
- **Relacionado a:** RF01, RF02, RF03, RF04, RF05, RF06, RF07, RF08, RF09 e RF10.

### RNF05 – Integridade dos dados
- **Descrição:** O sistema deverá manter os dados das tarefas consistentes após operações de cadastro, edição, exclusão e atualização de prioridade, prazo e status.
- **Categoria:** Confiabilidade
- **Prioridade:** Alta
- **Critério de verificação:** Verificar se as informações cadastradas ou alteradas são corretamente armazenadas e apresentadas nas consultas posteriores, sem alterações indevidas ou perda de dados.
- **Relacionado a:** RF03, RF04, RF05, RF06, RF07, RF08 e RF09.

## Considerações finais

Os requisitos não funcionais estabelecem critérios de qualidade que deverão ser considerados durante o desenvolvimento e a validação do TaskFlow. Eles complementam os requisitos funcionais, contribuindo para que o sistema seja seguro, confiável, simples de utilizar e compatível com os navegadores definidos.
