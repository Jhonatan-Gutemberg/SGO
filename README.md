# Sistema de Gestão das Olimpíadas (SGO)

__ __
> [!NOTE]
>  Autores: Jhonatan Gutemberg Rosa Ferreira e Gabriel Henrique Miranda Rodrigues

__ __

### Descrição do sistema:

 Com a chegada das Olimpíadas, um novo sistema de gestão é
necessário para coordenar os diferentes aspectos do evento. Este sistema deve permitir o
gerenciamento de competições, inscrições de atletas, alocação de locais para as provas,
e controle de resultados.
Regras de Negócio:
1. Cadastro de competições:
• O sistema deve permitir o cadastro de competições, que incluem o nome da
modalidade, data, horário, local e lista de atletas inscritos.
2. Inscrição de atletas:
• Atletas de diferentes países devem se inscrever em competições específicas.
Cada atleta pode participar de várias competições, mas só pode representar um
país em cada modalidade.
3. Alocação de locais:
• Os locais para as competições devem ser alocados de forma a evitar conflitos de
horário. Um local só pode abrigar uma competição por vez.
4. Controle de resultados:
• Após a realização das competições, os resultados devem ser registrados,
determinando o atleta vencedor e os classificados em segundo e terceiro lugares.
5. Relatórios de medalhas:
• O sistema deve gerar relatórios de medalhas, mostrando o desempenho de cada
país com base nas medalhas de ouro, prata e bronze conquistadas.

### Histórias de usuário

**US01: Cadastro de evento**
***Como*** organizador do evento,
***eu quero*** cadastrar evento,
***para que*** as datas, horários, locais sejam registrados de forma centralizada.

- ***Critérios de aceitação***:
  - O sistema deve permitir o cadastro de eventos, que incluem o nome da
modalidade, data, horário, local.
  

 
**US02: Editação de evento**
***Como*** organizador do evento,
***eu quero*** editar evento,
***para que*** as datas, horários, locais sejam alterados de forma centralizada.

**US03: Remoção de Evento**
***Como*** organizador do evento,
***eu quero*** remover um evento do sistema,
***para que*** ele não apareça mais nas programações e registros centralizados.

**US04: Gerenciar Inscrições**
***Como*** organizador do evento,
***eu quero*** gerenciar as inscrições dos atletas,
***para*** que eu possa adicionar, editar ou remover inscrições de competições de forma centralizada. 

**US05: Inscrição do Atleta em Competição**
***Como*** atleta,  
***eu quero*** me inscrever em uma competição,  
***para que*** eu possa participar do evento e representar meu país.

- ***Critérios de aceitação***:
  - O sistema deve permitir que o atleta selecione a modalidade e a competição desejada.
  - Atletas de diferentes países devem se inscrever em competições específicas.
Cada atleta pode participar de várias competições, mas só pode representar um
país em cada modalidade.
  - O sistema deve garantir que o atleta só pode representar um país em cada modalidade.
  - Após a inscrição, o sistema deve enviar uma confirmação ao atleta.
  

**US06: Consultar Resultado de Competição**
***Como*** atleta,  
***eu quero*** consultar o resultado de uma competição,  
***para que*** eu possa ver o desempenho dos atletas e os vencedores.

- **Critérios de aceitação**:
  - O sistema deve permitir a pesquisa de competições por nome, data ou modalidade.
  - O sistema deve exibir os três primeiros colocados (1º, 2º e 3º lugares) com seus respectivos tempos/pontuações.
  - O sistema deve exibir os resultados para todos os atletas que participaram da competição.

**US07: Consultar Dados do Evento**
***Como*** atleta ou espectador,  
***eu quero*** consultar os dados de um evento,  
***para que*** eu possa obter informações sobre datas, horários, locais e competições associadas.

- **Critérios de aceitação**:
  - O sistema deve permitir a busca de eventos por nome, data ou local.
  - O sistema deve exibir a lista de competições associadas ao evento, com suas respectivas modalidades, horários e locais.
  - O sistema deve mostrar a lista de atletas inscritos em cada competição.
  - O sistema deve estar atualizado em tempo real com quaisquer alterações nos eventos.

**US08: Registrar Pontuação**
***Como*** árbitro,
***eu quero*** registrar a pontuação de uma competição,
***para que*** os resultados sejam armazenados corretamente e possam ser consultados posteriormente.

**US09: Manutenir Provas**
***Como*** árbitro,  
***eu quero*** manutenir as provas,  
***para que*** eu possa atualizar ou remover provas quando necessário.

- **Critérios de aceitação**:
  - O sistema deve permitir a edição de detalhes da prova, como datas, horários, locais e atletas inscritos.
  - O sistema deve permitir a remoção de provas canceladas ou alteradas, solicitando uma confirmação antes da exclusão.
  - O sistema deve validar que, ao editar uma prova, não existam conflitos de horário ou local.
  
**US10: Alocar Local de Competição**
***Como*** membro do Comitê Olímpico,
***eu quero*** alocar locais para as competições,
***para que*** cada competição tenha um local adequado sem conflitos de horário.

- **Critérios de aceitação**:
    - O sistema deve permitir o cadastro de competições, que incluem o nome da
modalidade, data, horário, local e lista de atletas inscritos.
    - O sistema deve verificar se o local escolhido está disponível no horário desejado e não possui conflitos com outras competições.
  
**US11: Manter Data e Horário da Competição**
***Como*** membro do Comitê Olímpico,  
***eu quero*** realizar a manutenção das datas e horários das competições,  
***para que*** eu possa ajustar o cronograma conforme necessário.

- **Critérios de aceitação**:
  - O sistema deve permitir a edição das datas e horários de competições já cadastradas.
  - O sistema deve garantir que não haja conflitos de horário entre competições no mesmo local.
  - O sistema deve registrar todas as mudanças feitas, incluindo o responsável, data e hora da alteração.
  - O sistema deve notificar os atletas e organizadores sobre alterações no cronograma.
  - O sistema deve exibir uma visualização completa do cronograma antes e depois de realizar alterações, mostrando o impacto no restante das competições.

**US12: Apresentar Desempenho por País**
***Como*** membro da Federação Olímpica,
***eu quero*** apresentar o desempenho dos países,
***para que*** seja possível visualizar o total de medalhas conquistadas por cada país.

- **Critérios de aceitação**:
  - O sistema deve exibir o total de medalhas de ouro, prata e bronze conquistadas por cada país.

**US13: Cadastrar Competição**
***Como*** membro da Federação Olímpica,  
***eu quero*** cadastrar uma nova competição,  
***para que*** ela seja adicionada ao calendário oficial das Olimpíadas.

- **Critérios de aceitação**:
  - O sistema deve permitir a inserção de todos os detalhes da competição, incluindo modalidade, data, horário e local.

**US14: Cancelar Competição**
***Como*** membro da Federação Olímpica,  
***eu quero*** cancelar uma competição,  
***para que*** ela seja removida do cronograma e os atletas sejam informados.

- **Critérios de aceitação**:
  - O sistema deve permitir a busca e seleção de uma competição para cancelamento.
  
**US15: Consultar Competição**
***Como*** membro da Federação Olímpica,  
***eu quero*** consultar as informações de uma competição,  
***para que*** eu possa visualizar detalhes como horário, local, atletas inscritos e resultados.

- **Critérios de aceitação**:
  - O sistema deve permitir a busca por nome, data, modalidade ou local da competição.
  - O sistema deve exibir todos os detalhes da competição, incluindo horário, local, atletas inscritos e resultados (caso já finalizada).

**US16: Login**
***Como*** usuário,
***eu quero*** realizar login,
***para que*** eu posso ter acesso as informção do meu nível de responsabilidade.

- **Critérios de aceitação**:
  -O sistema de ser capaz de escalar responsabilidade aos usários
  
__ __

>### Diagrama de caso de uso


<img width="741px" height="741px" src="img\Diagrama de caso de uso.png"/>

__ __

>### Diagrama depacotes



<img width="8760px" height="460px" src="img\Diagrama de pacotes Otimizado.png"/>

>### Diagrama de Implantação e Componentes
![image](https://github.com/user-attachments/assets/51f37800-e748-4213-b3d9-ee5d8a10d49e)

