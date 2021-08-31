<h1 align="center" style="color:#0091EA; font-weight:bold;">
     <img 
    src="https://user-images.githubusercontent.com/42190754/131585039-5a08a2f0-d675-4ec7-97af-32b98c6d337c.png"
    float="center"
    width="100" height="100"
    />
    <br/>
  <a href="#"> Algoritmo A* </a>
</h1>

## ℹ️ Sobre

- [x] Algoritmo guloso
- [x] encontra o menor caminho de maneira super eficiente.
- [x] Requer definição de uma função heurística h(x), que subestima a distância entre o vértice x e o vértice destino.
- [x] A ideia por trás do A* é transformar o grafo em uma árvore
- [x] A raiz da árvore é o nó origem
- [x] Essa árvore será estendida a partir de suas folhas (que no começo é só o nó origem), usando o grafo como referência
- [x] Não vai expandir todas as possibilidades, apenas as que parecerem mais promissoras

---

### 💠 Como saber se uma possibilidade é promissora?
* Através da função F(x) = g(x) + h(x)
    * Que é uma função heurística
        * g(x) é o custo para, a partir da origem, chegar até o nó x
        * h(x) é uma função heurística para a estimativa do custo do próximo nó
    * Sempre olhamos as possibilidades de expansão da árvore e calculamos o valor de F(x)
        * Adicionamos o nó que possui o menor F(x) dentre os que encontramos
---

* O A* é o algoritmo mais eficiente para caminhos mínimos em grafos
* Entretanto, ele limitações severas
  * É preciso definir uma h(x) que seja admissível: ela nunca irá retornar um valor maior do que a distância real de x até y
  * Se h(x) for admissível, mas subestimar demais a distância real, o algoritmo fica super ineficiente. Se h(x) não for admissível, o algoritmo poderá não encontrar o caminho mínimo

---

## 📈 Complexidade
* A complexidade depende diretamente da função h(x) usada.
* No pior caso, a quantidade de nós explorados é exponencial no tamanho do menor caminho, mas tem complexidade polinomial se h∗(x)−h(x)≤O(logh∗(x)).

---
### 💠 Quando é bom usar?
* Grafos onde se pode subestimar a distância entre dois vértices, como em mapas
* A menor distância entre dois pontos é uma reta, mas provavelmente a distância real será maior que isso

---

## 🤔 Qual é o caminho mínimo nesse caso?

<p align="center" style="display: flex; align-items: flex-start; justify-content: center; margin:5px">
      <img style="margin:5px" alt="spaceDetail" src="https://user-images.githubusercontent.com/42190754/131263989-c6597398-b49b-4862-a5bb-a589774ee899.png" width="600px">
</p>

---

## 🚀 Executar o projeto
<details>
  <summary>Resultado</summary>
<p align="center" style="display: flex; align-items: flex-start; justify-content: center; margin:5px">
      <img style="margin:5px" alt="spaceDetail" src="https://user-images.githubusercontent.com/42190754/131263973-424a5f60-47e5-4dec-91c9-df6779806c75.png" width="600px">
</p>
</details>

---

## 👩🏽‍💻 Autores

<table>
  <tr>
    <td align="center"><a href="https://github.com/biachacon"><img src="https://avatars1.githubusercontent.com/u/42190754?s=460&u=a5cbe42a4868b2bac9615226044b9cec15cee418&v=4" width="100px;" alt=""/><br /><sub><b>Bia Chacon</b></sub></a><br /><a href="https://github.com/BiaChacon/a-star-algorithm" title="Code">💻</a></td>
  <tr>
</table>

---

## 📝 Licença

Este projeto está sob o MIT. Veja aqui [LICENSE](https://github.com/BiaChacon/a-star-algorithm/blob/main/LICENSE) para mais informações.

---