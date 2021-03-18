---
title: CTT
sections:
   - Modelo CTT
---

#### Um pouco sobre o CTT:

O CTT (ConcurTaskTrees/Árvores  de  Tarefas  Concorrentes) foi  criado  para auxiliar a avaliação e o design e avaliação de IHC (Paternò, 2000). Estabelecendo hierarquia entre as taferas a fim de garantir a completa execução de determinada operação.

### Modelo CTT:

Nesse modelo, existem quatro tipos de tarefas:

* tarefas do usuário, realizadas fora do sistema; 
* tarefas do sistema, em que o sistema realiza um processamento sem interagir com o usuário; 
* tarefas interativas, em que ocorrem os diálogos usuário–sistema; 
* tarefas  abstratas, que não são tarefas em si, mas sim uma representação de uma composição de tarefas que auxilie a decomposição.

Além da hierarquia, o CTT permite representar diversas relações entre as tarefas, que aumentam  a  expressividade  da  notação.

<div class="screenshot-holder" style="display: flex; justify-content: center;">
<a href="assets/images/taregas_CTT.PNG" data-title="Tarefas CTT" data-toggle="lightbox">
<img class="img-responsive" src="assets/images/taregas_CTT.PNG" alt="screenshot" style="width: 100%" />
</a>
<a class="mask" href="assets/images/taregas_CTT.PNG" data-title="Tarefas CTT" data-toggle="lightbox">
<i class="icon fa fa-search-plus"></i>
</a>
</div>
Fonte: BARBOSA. SILVA, 2010, P.204

Os  significados  dessas  relações  são os seguintes:

* ativação: T1 >> T2: (T2) só inicia após (T1) terminar
* ativação  com  passagem  de  informação: T1  [  ]  >>  T2  igual a anterior com a adição da informação produzida por T1 ser passada para T2;
* escolha (tarefas alternativas): T1 [] T2: Quando uma das tarefas for habilitada a outra será desabilitada;
* tarefas  concorrentes: T1 ||| T2 : as tarefas podem ser realizadas em qualquer ordem ou ao mesmo tempo;
* tarefas concorrentes e comunicantes: T1 | [ ] | T2 igual a anterior com adição de troca de informações;
* tarefas independentes: T1 |=| T2 as tarefas podem ser realizadas em qualquer ordem, mas quando uma delas é iniciada, precisa terminar para que a outra possa ser iniciada;
* desativação: T1  [>  T2  especifica que T1  é  completamente  interrompida  por  T2;
* suspensão/retomada: T1 |> T2 especifica que T1 pode ser interrompida por T2 e é retomada do ponto em que parou assim que T2 terminar.

A grande vantagem de se usar o CTT é a possibilidade do registro explícito das relações entre as tarefas.