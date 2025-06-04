````markdown
# 🎂 Simulação do Paradoxo do Aniversário

Este projeto é uma simulação do famoso **Paradoxo do Aniversário**, que mostra como é surpreendentemente provável que duas pessoas em um grupo compartilhem a mesma data de aniversário. A simulação utiliza o método de Monte Carlo para gerar milhares de cenários aleatórios e calcular essa probabilidade.

## 📋 Descrição

Apesar de parecer improvável, em um grupo de apenas 23 pessoas, a chance de pelo menos duas delas fazerem aniversário no mesmo dia é de cerca de 50%. Este programa demonstra esse fenômeno por meio de simulações repetidas.

O código:

- Gera uma quantidade especificada de aniversários aleatórios.
- Verifica se há alguma coincidência entre eles.
- Repete esse processo 100.000 vezes para estimar a probabilidade de coincidências.

## 🚀 Como usar

1. Execute o script Python.
2. Digite o número de aniversários a serem gerados (entre 1 e 100).
3. O programa mostrará os aniversários gerados e se houve coincidência.
4. Em seguida, ele executará 100.000 simulações para calcular a probabilidade.

### Exemplo de uso:
```bash
$ python birthday_paradox.py
How many birthdays shall I generate? (Max 100)
> 23
````

## 📦 Dependências

* Python 3
* Módulos padrão:

  * `datetime`
  * `random`

## 🧠 Conceitos envolvidos

* **Paradoxo do Aniversário:** Um resultado contra-intuitivo da teoria das probabilidades.
* **Simulação de Monte Carlo:** Técnica de simulação estatística usada para estimar resultados baseados em repetições aleatórias.

## 📁 Estrutura do código

* `getBirthdays(n)`: Gera `n` datas aleatórias de aniversário.
* `getMatch(birthdays)`: Verifica se há algum aniversário duplicado na lista.
* Laço principal: Interage com o usuário e realiza as simulações.

## 📊 Resultado esperado

O programa exibirá algo como:

```
Out of 100,000 simulations of 23 people, there was a
matching birthday in that group 50716 times. This means
that 23 people have a 50.72% chance of
having a matching birthday in their group.
That's probably more than you would think!
```
