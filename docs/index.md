<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>


<font size="+12"><center>
## Be Present
</center></font>



**Conteúdo**

- [Autores](#nome-alunos)
- [Descrição do projeto](#introdução-do-projeto)
- [Análise de requisitos funcionais e não-fucionais](#descrição-dos-requisitos)
- [Diagrama de casos de uso](#diagrama-de-comportamento-atores)
- [Descrição dos casos de uso](#descrição-das-funcões)
- [Diagrama de senquencia](#diagrama-de-ordem-interações)
- [Diagrama de classes](#diagrama-orientado-objetos)
- [Diagrama de componentes](#diagrama-estrutura-componente)
- [Decisões de arquitetura](#decisões-de-arquitetura)
- [Diagrama de implantação](#diagrama-de-hardware-software)
- [Referências](#referências)


# Autores

* Matteo Domiciano Varnier
* Felipe Mazzeo Barbosa 
* Daniel Reis Raske



# Descrição do projeto

*A Escola Infinito necessita de um sistema para controlar as presenças de seus
alunos, pois a operação ainda é realizada totalmente em papel.*

# Análise de requisitos funcionais e não-funcionais
### Requisitos Funcionais:

1. Permitir que professores registrem duas faltas de forma fácil e intuitiva.

2. Facilitar a análise e o acompanhamento do número de faltas.

3. Enviar notificações por e-mail aos pais ou responsáveis quando a porcentagem de presencas estiverem abaixo de 80%.

4. Gerar relatórios de faltas, permitindo o agrupamento por data, ano do ensino, turma, professor, disciplina e aluno.

### Requisitos nao-FuncionaisL:

1. O sistema deve ser implementado com linguagem HTML, CSS, JS

2. O sistema deve ser executado tanto na WEB quanto em celular

3. O sistema deve ser relacionado com um banco de dados

4. O sistema deve suportar muitos acessos simultaneos.

# Diagrama de casos de uso

![alt](/assets/Caso_e_uso.png)

# Descrição dos casos de uso
### Registrar Falta:

**Ator: Professor, ADM Sistema**

**Descrição: O professor registra a falta de um determinado aluno em uma aula/dia específico.**

**Fluxo básico:**

- O professor acessa a funcionalidade "Registrar Falta".
- O sistema apresenta a lista de turmas e alunos.
- O professor seleciona a turma e o aluno que faltou.
- O professor registra a falta do aluno na data atual.
- O sistema salva a informação de falta registrada.
- ADM Sistema visualiza se ocorreu alguma falta 
- O ADM ve se registra no site as faltas

### Relatório de Faltas:

**Ator: Professor, ADM Sistema**

**Descrição: Gera um relatório com informações consolidadas sobre as faltas.**

**Fluxo básico:**
- O usuário acessa a funcionalidade "Gerar Relatório de Faltas".
- O sistema apresenta filtros de busca (aluno, turma, data, disciplina etc).
- O usuário seleciona os filtros desejados.
- O sistema gera o relatório de acordo com os filtros.
- O usuário visualiza o relatório de faltas gerado.

### Notificação:

**Ator: Professor, Pais/Responsaveis, ADM Sistema**

**Descrição: Envia uma notificação por e-mail aos pais/responsáveis sobre a situação de faltas do aluno.**

 **Fluxo básico:**
- O sistema verifica diariamente o percentual de faltas de cada aluno.
- Para alunos com percentual abaixo do limite definido, o sistema automaticamente aciona o caso de uso "Enviar Notificação".
- O sistema busca os dados de e-mail dos pais/responsáveis.
- O sistema envia a notificação por e-mail

### Acessibilidae:

**Ator: ADM Sistema**

**Descrição: Permite configurar as opções de acessibilidade e outras configurações do sistema.**

**Fluxo básico:**
- O administrador acessa a tela de configurações do sistema.
- O administrador altera as configurações de fonte, contraste, notificações, entre outras.
- O sistema salva as configurações aplicadas.

## Qualquer Site/WEB:

**Ator: Professor, Adm Sistema, Pais/Responsaveis**

**Descrição: Permite configurar as opções de acessibilidade e outras configurações do sistema.**

**Fluxo básico:**
- O administrador acessa a tela de configurações do sistema.
- O administrador coloca todas as faltas no sistema.
- O sistema envia notificacao por aplicativo ou pelo site
- Professores e pais podem acessar o site pelo ID do aluno ou ID do professor
- Pais e professores veem a quantidade de falta
- Pais podem justificar a falta dos filhos com atestado


# Diagrama de sequencia

*&lt;Descrição do comportamento entre os atores/resquisitos&gt;*

# Diagrama de classes

*&lt;Diagrama de relacionamento entre classes para os seus atributos e operações&gt;*

# Diagrama de Componentes

*&lt;Diagrama para exibir a relação estrutural dos componentes de um sistema de software

# Decisões de arquitetura

*&lt;Descrever a infraestrutura escolhida para arquitetura do projeto&gt;*

# Diagrama de implantação

*&lt;Diagrama para exibir o relacionamento de hardware e software no projeto&gt;*

# Referências

*&lt;Lista de referências&gt;*
