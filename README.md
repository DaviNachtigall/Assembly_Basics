# Neander Assembly - Integer Division

This repository contains an 8-bit Assembly algorithm developed for the **Neander** simulator architecture. 

The program divides value **A** by value **B** using **successive subtractions**, storing the quotient in **RESULT** and the remainder in **RESTO**.

---

## Code Preview

<img width="602" height="562" alt="image" src="https://github.com/user-attachments/assets/6df4af2d-9472-4272-89ec-a33861890967" />


---

## How it Works

1. **Two's Complement:** It applies a bitwise `NOT` to `B` and adds `UM` (1) to make it negative (`NB`).
2. **Subtraction Loop:** It repeatedly adds `NB` to `A` ($A = A - B$).
3. **Logic:** The loop continues until the result turns negative (`JN FIM`), incrementing `RESULT` on each successful step.
4. **Output:** The final positive remainder is saved in `RESTO`.

## Initial Variables (Example)
* `A`: `#12` (Dividend)
* `B`: `#04` (Divisor)
* `RESULT`: stores $12 \div 4 = \mathbf{3}$
* `RESTO`: stores $12 \pmod 4 = \mathbf{0}$
