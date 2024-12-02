# Simulação do Algoritmo Raft em Python

Este projeto implementa uma simulação do algoritmo de consenso **Raft**, amplamente utilizado em sistemas distribuídos. O objetivo é demonstrar como um cluster distribuído alcança consenso mesmo na presença de falhas simuladas de nós.

---

## **Descrição do Projeto**

O algoritmo **Raft** é uma abordagem simplificada e intuitiva para resolver o problema do consenso em sistemas distribuídos. Ele organiza os nós em três estados principais:  
- **Follower (seguidor):** Recebe comandos de um líder.  
- **Candidate (candidato):** Compete para se tornar líder.  
- **Leader (líder):** Coordena o cluster e replica os logs.  

Nesta implementação, simulamos os seguintes aspectos:  
- **Eleição de líder:** Os nós competem para se tornar líder quando necessário.  
- **Replicação de logs:** O líder distribui informações para os seguidores.  
- **Falhas e recuperação:** Simulamos falhas aleatórias e recuperações de nós, validando a robustez do sistema.  

---

## **Estrutura do Código**

- **src/cluster.py:** Gerencia o cluster e controla a interação entre os nós.  
- **src/node.py:** Contém a lógica de comportamento de cada nó, incluindo eleição, replicação e comunicação.  
- **src/main.py:** Ponto de entrada para executar o sistema.  
- **tests/test_cases.md:** Documentação dos cenários de teste utilizados.  
- **requirements.txt:** Lista as dependências do projeto.  
