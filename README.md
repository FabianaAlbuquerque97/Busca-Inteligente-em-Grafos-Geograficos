# Busca Inteligente em Grafos Geográficos

Este projeto implementa um agente inteligente capaz de encontrar a rota de menor custo entre duas cidades dos Estados Unidos. Com base em dados geográficos (latitude e longitude) e populacionais, o agente constrói um grafo de conexões diretas entre cidades e aplica algoritmos de busca para determinar o caminho mais eficiente entre dois pontos, considerando critérios como distância e população.

---

## 🧠 Modelo PEAS

| Componente     | Descrição |
|----------------|-----------|
| **Performance** | Menor distância total entre origem e destino; prioridade para cidades com menor população em caso de empate. |
| **Environment** | Conjunto de cidades (nós) conectadas por estradas (arestas) quando a distância ≤ `r`, com base na distância euclidiana. |
| **Actuators**   | Escolha da próxima cidade, atualização do caminho atual, visualização do grafo e do caminho. |
| **Sensors**     | Leitura dos dados geográficos e populacionais do arquivo JSON, cálculo de distâncias e raio `r`. |

---

## 🚀 Tecnologias utilizadas

- Python 3
- NetworkX
- Matplotlib
- JSON
- Heapq (fila de prioridade)
