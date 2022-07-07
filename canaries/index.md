## Uma aplicação que será utilizada por jogadores amadores de tenis.

- Estes jogadores fazem parte de um ranking que é atualizado conforme a realização das partidas
- Atualmente este ranking é controlado de forma manual, e o organizador nos procurou para que possamos desenvolver uma aplicação que venha modenizar este controle, visando incentivar quem já participa, bem como disponibilizar um atrativo para novos jogadores

---

### Jogador

- Solicitar ou rejeitar um desafio
- Registrar o resultado de uma partida
- Acompanhar os rankings
- Consultar seus dados e seu histórico de partidas(vitória, derrotas posição no ranking)
- Consultar as informações de seus adversários (histórico de partidas e dados)
- Ser notificado por e-mail quando desafiado

### Administrador

- Cadastrar as categorias e definir as pontuações
- Cadastrar jogadores e definir suas categorias
- Ser notificado quando existir um desafio pendente a mais de 10 dias

---

### Entidades 

- Categorias
- Jogadores
- Desafios
- Partidas
- Rankings
- Notificações


#### Categorias.

| _id                                  | categoria | descricao   | eventos.0.nome | eventos.0.operacao | eventos.0.valor | eventos.1.nome | eventos.1.operacao | eventos.1.valor | eventos.2.nome | eventos.2.operacao | eventos.2.valor | jogadores.0._id                      | jogadores.1._id                      |
| ------------------------------------ | --------- | ----------- | -------------- | ------------------ | --------------- | -------------- | ------------------ | --------------- | -------------- | ------------------ | --------------- | ------------------------------------ | ------------------------------------ |
| 534e5168-8baf-11ea-bc55-0242ac130003 | A         | Categoria A | VITORIA        | +                  | 30              | VITORIA_LIDER  | +                  | 50              | DERROTA        | +                  | 0               | 534e5168-8baf-11ea-bc55-0242ac130003 | f27263d6-8bb6-11ea-bc55-0242ac130003 |


#### Jogadores

| _id                                  | telefoneCelular | email                           | nome        | urlFotoJogador             | desempenho.0.categoria | desempenho.0.vitorias | desempenho.0.derrotas | desempenho.0.pontos | desempenho.1.categoria | desempenho.1.vitorias | desempenho.1.derrotas | desempenho.1.pontos |
| ------------------------------------ | --------------- | ------------------------------- | ----------- | -------------------------- | ---------------------- | --------------------- | --------------------- | ------------------- | ---------------------- | --------------------- | --------------------- | ------------------- |
| 534e5168-8baf-11ea-bc55-0242ac130003 | +5511994604784  | diegofsilva.fernandes@gmail.com | Diego Silva | www.google.com.br/foto.jpg | A                      | 5                     | 1                     | 100                 | B                      | 30                    | 5                     | 1200                |


#### Desafios

| _id                                  | dataHoraDesafio     | status    | dataHoraSolicitacao | dataHoraResposta    | solicitante                          | categoria | jogadores.0._id                      | jogadores.1._id                      | partida._id                          | partida.def                          | partida.resultado.0.set | partida.resultado.1.set | partida.jogadores.0._id              | partida.jogadores.1._id              |
| ------------------------------------ | ------------------- | --------- | ------------------- | ------------------- | ------------------------------------ | --------- | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ----------------------- | ----------------------- | ------------------------------------ | ------------------------------------ |
| 1f35042a-8bba-11ea-bc55-0242ac130003 | 2020-05-04 18:00:00 | REALIZADO | 2020-04-25 08:30:00 | 2020-04-26 08:30:00 | 534e5168-8baf-11ea-bc55-0242ac130003 | A         | 534e5168-8baf-11ea-bc55-0242ac130003 | f27263d6-8bb6-11ea-bc55-0242ac130003 | 1f35042a-8bba-11ea-bc55-0242ac130003 | 534e5168-8baf-11ea-bc55-0242ac130003 | 6-1                     | 6-3                     | 534e5168-8baf-11ea-bc55-0242ac130003 | f27263d6-8bb6-11ea-bc55-0242ac130003 |


#### Partidas 

| _id                                  | def                                  | resultado.0.set | resultado.1.set | jogadores.0._id                      | jogadores.1._id                      |
| ------------------------------------ | ------------------------------------ | --------------- | --------------- | ------------------------------------ | ------------------------------------ |
| 1f35042a-8bba-11ea-bc55-0242ac130003 | 534e5168-8baf-11ea-bc55-0242ac130003 | 6-1             | 6-3             | 534e5168-8baf-11ea-bc55-0242ac130003 | f27263d6-8bb6-11ea-bc55-0242ac130003 |


#### Rankings


| desafio | partida | categoria | jogador                              | evento  | operacao | pontos |
| ------- | ------- | --------- | ------------------------------------ | ------- | -------- | ------ |
|         |         | A         | 534e5168-8baf-11ea-bc55-0242ac130003 | VITORIA | +        | 100    |

---