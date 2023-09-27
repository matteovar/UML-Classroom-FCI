<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Ciencia da Computação</a></h3>


<font size="+12"><center>
## Be Present
</center></font>


**Conteúdo**

- [Autores](#autores)
- [Descrição do projeto](#Descrição-do-projeto)
- [Análise de requisitos funcionais e não-fucionais](#Análise-de-requisitos-funcionais-e-não-funcionais)
- [Diagrama de casos de uso](#Diagrama-de-casos-de-uso)
- [Descrição dos casos de uso](#Descrição-dos-casos-de-uso)
- [Diagrama de senquencia](#Diagrama-de-sequencia)
- [Diagrama de classes](#Diagrama-de-classes)
- [Diagrama de componentes](#Diagrama-de-Componentes)
- [Decisões de arquitetura](#Decisões-de-arquitetura)
- [Diagrama de implantação](#Diagrama-de-implantação)
- [Referências](#Referências)


# Autores

* Matteo Domiciano Varnier
* Felipe Mazzeo Barbosa 
* Daniel Reis Raske



# Descrição do projeto

*A Escola Infinito necessita de um sistema para controlar as presenças de seus
alunos, pois a operação ainda é realizada totalmente em papel.*

# Análise de requisitos funcionais e não-funcionais
### Requisitos Funcionais:

1. Permitir que professores registrem faltas de forma fácil e intuitiva.

2. O sistema deve ser capaz de gerar relatórios de faltas, permitindo o agrupamento por data, ano do ensino, turma, professor, disciplina e aluno. 

3. Facilitar a análise e o acompanhamento do número de faltas.

4. Enviar notificações por e-mail aos pais ou responsáveis quando a porcentagem de comparecimento às aulas estiver abaixo de 80%.

### Requisitos nao-funcionais:

1. O sistema deve ser implementado em lingugem HTML, CSS e JS
2. O sistema devera ser interligado com um banco de dados
3. O sistema devera ser funcional tanto na WEB quando mobile
4. O usuario devera ser capaz de suportar varios acessos simultaneos
5. O usuario devera escolher uma senha forte com no minimo 6 digitos, 1 caractere especial e 1 letra maiuscula. 

# Diagrama de casos de uso

![alt](/assets/Caso_e_uso.png)

# Descrição dos casos de uso

### Registrar Falta:

**Ator: Professor**

**Descrição: O professor registra a falta de um determinado aluno em uma aula/dia em dois momentos diferentes.**

**Fluxo básico:**

- O professor acessa a funcionalidade "Registrar Falta".
- O sistema apresenta a lista de turmas e alunos.
- O professor seleciona a turma e o aluno que faltou.
- O professor registra a falta do aluno na data atual.
- O sistema salva a informação de falta registrada.

### Relatório de Faltas:

**Ator: Professor**

**Descrição: Gera um relatório com informações consolidadas sobre as faltas.**

**Fluxo básico:**
- O usuário acessa a funcionalidade "Gerar Relatório de Faltas".
- O sistema apresenta acessibilidade de busca (aluno, turma, data, disciplina, professor).
- O usuário seleciona os filtros desejados.
- O sistema gera o relatório de acordo com os filtros.
- O usuário visualiza o relatório de faltas gerado.
- O ususario visuzaliza a porcentagem de falta

### Notificação:

**Ator:Pais/Responsaveis**

**Descrição: Envia uma notificação por e-mail aos pais/responsáveis sobre a situação de faltas do aluno.**

 **Fluxo básico:**
- O sistema verifica diariamente o percentual de faltas de cada aluno.
- Para alunos com percentual abaixo do limite definido, o sistema automaticamente aciona o caso de uso "Enviar Notificação".
- O sistema busca os dados de e-mail dos pais/responsáveis.
- O sistema envia a notificação por e-mail

### Acessibilidae:

**Ator: Sistema**

**Descrição: Permite configurar as opções de acessibilidade e outras configurações do sistema.**

**Fluxo básico:**
- O administrador acessa a tela de configurações do sistema.
- O administrador altera as configurações de fonte, contraste, notificações, entre outras na WEB ou no mobile
- O sistema salva as configurações aplicadas.
- O sistema permite modificar o registro de faltas

### Qualquer Site/WEB:

**Ator: Professor, Adm Sistema, Pais/Responsaveis**

**Descrição: Permite configurar as opções de acessibilidade e outras configurações do sistema.**

**Fluxo básico:**
- O administrador acessa a tela de configurações do sistema.
- O administrador coloca todas as faltas no sistema.
- No sistema é possivel visualizar as notificacoes por aplicativo ou pelo site
- Professores e pais podem acessar o site pelo ID do aluno ou ID do professor
- Pais e professores veem a quantidade de falta
- Pais podem justificar a falta dos filhos com atestado



# Diagrama de sequencia

- Diagrama de sequencia da (sistema de chamada)

![alt](/assets/chamada.png)

-Diagrama de Sequencia (gera Relatorio)

![alt](/assets/Gera_Relatorio.png)

-Diagrama de Sequencia (email automatico relatorio)

![alt](/assets/Email_auto.png)


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
