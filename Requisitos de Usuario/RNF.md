# Requisitos Não Funcionais – TaskFlow

## Introdução

Este documento apresenta os requisitos não funcionais do TaskFlow, definindo critérios de qualidade, segurança, desempenho e usabilidade do sistema.

## Requisitos

### RNF01 – Usabilidade
- **Descrição:** O sistema deverá apresentar uma interface simples e intuitiva, permitindo que os usuários encontrem as principais funcionalidades sem dificuldades.
- **Categoria:** Usabilidade
- **Prioridade:** Alta
- **Critério de verificação:** Verificar se um usuário consegue cadastrar, editar e consultar uma tarefa sem precisar de instruções externas.
- **Relacionado a:** RF03, RF04 e RF09.

### RNF02 – Desempenho
- **Descrição:** O sistema deverá responder às operações de consulta e cadastro de tarefas em até 3 segundos em condições normais de uso.
- **Categoria:** Desempenho
- **Prioridade:** Alta
- **Critério de verificação:** Medir o tempo de resposta das operações de cadastro e consulta.
- **Relacionado a:** RF03 e RF09.

### RNF03 – Segurança
- **Descrição:** O sistema deverá proteger o acesso às informações dos usuários, permitindo que cada usuário acesse somente seus próprios dados.
- **Categoria:** Segurança
- **Prioridade:** Alta
- **Critério de verificação:** Testar se um usuário consegue acessar informações pertencentes a outra conta.
- **Relacionado a:** RF01 e RF02.

### RNF04 – Compatibilidade
- **Descrição:** O sistema deverá funcionar nos principais navegadores modernos, como Google Chrome, Mozilla Firefox e Microsoft Edge.
- **Categoria:** Compatibilidade
- **Prioridade:** Média
- **Critério de verificação:** Testar as funcionalidades principais nos navegadores indicados.
- **Relacionado a:** RF03, RF04 e RF09.

### RNF05 – Integridade dos dados
- **Descrição:** O sistema deverá manter os dados das tarefas consistentes após operações de cadastro, edição e exclusão.
- **Categoria:** Confiabilidade
- **Prioridade:** Alta
- **Critério de verificação:** Verificar se as alterações realizadas nas tarefas são corretamente refletidas nas consultas posteriores.
- **Relacionado a:** RF03, RF04 e RF05.

## Considerações finais

Os requisitos não funcionais estabelecem critérios de qualidade que deverão ser considerados durante o desenvolvimento e a validação do TaskFlow.
