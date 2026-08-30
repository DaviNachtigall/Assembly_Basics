# Neander Assembly - Divisão de Inteiros
Este repositório contém um algoritmo em Assembly de 8 bits desenvolvido para a arquitetura do simulador **Neander**. 
O programa divide o valor **A** pelo valor **B** usando **subtrações sucessivas**, armazenando o quociente em **RESULT** e o resto em **RESTO**.

---

## Prévia do Código
<img width="602" height="562" alt="image" src="https://github.com/user-attachments/assets/6df4af2d-9472-4272-89ec-a33861890967" />

---

## Como Funciona
1. **Complemento de Dois:** Aplica-se uma operação bit a bit `NOT` em `B` e soma-se `UM` (1) para torná-lo negativo (`NB`).
2. **Laço de Subtração:** Soma-se repetidamente `NB` a `A` ($A = A - B$).
3. **Lógica:** O laço continua até que o resultado se torne negativo (`JN FIM`), incrementando `RESULT` a cada etapa bem-sucedida.
4. **Saída:** O resto positivo final é salvo em `RESTO`.

## Variáveis Iniciais (Exemplo)
* `A`: `#12` (Dividendo)
* `B`: `#04` (Divisor)
* `RESULT`: armazena $12 \div 4 = \mathbf{3}$
* `RESTO`: armazena $12 \bmod 4 = \mathbf{0}$
