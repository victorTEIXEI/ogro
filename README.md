# Idade de Camila – OBI (Olimpíada Brasileira de Informática)

**Dupla:** [Victor Teixeira Nascimento] e [Denys Celso Leal Reis]  
**Disciplina:** Introdução a Computação  
**Etapa:** 3ª Etapa  
**Ano da questão:** [OBI 2021 – Programção Nível Júnior – Fase 1]

---

## 📝 Descrição da Questão

Cibele, Camila e Celeste são três irmãs. Sabemos que:

- Cibele nasceu **antes** de Camila (é a mais velha);
- Celeste nasceu **depois** de Camila (é a mais nova).

Portanto, Camila é a irmã do meio em idade.

A entrada contém três números inteiros (idades), um por linha. O programa deve determinar qual dessas idades pertence a Camila e imprimi-la.

**Exemplo de entrada:**
15
10
20

**Exemplo de saída:**
15

**Explicação:** As idades fornecidas são 15, 10 e 20. Após ordenação, temos 10 (Celeste, a mais nova), 15 (Camila, a do meio) e 20 (Cibele, a mais velha). Logo, a idade de Camila é 15.

---

## 🧠 Raciocínio da Solução

Independentemente de qual número corresponde a cada irmã, a idade de Camila será sempre o **valor mediano** (o do meio) entre os três números lidos.

**Lógica:**
1. Ler as três idades.
2. Armazenar em uma lista.
3. Ordenar a lista em ordem crescente.
4. O valor da posição central (índice 1) é a idade de Camila.

---

## 💻 Código-fonte (Python)

```python
id1 = int(input(""))
id2 = int(input(""))
id3 = int(input(""))
L = []
L.append(id1)
L.append(id2)
L.append(id3)
L.sort()
print(L[1])
