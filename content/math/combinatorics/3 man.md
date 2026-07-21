---
title: "3-man"
date: 2026-07-21
draft: false
---

### Puzzle 2

#### Puzzle Statement

There are $100$ soldiers in a detachment, and every evening three of them are on duty. Can it happen that, after a certain period of time, each soldier has shared duty with every other soldier exactly once?

#### Solution

**Difficulty:** Easy.  
**Hint:** Parity.

**Comment:** This took me embarrassingly long to figure out. It's a cute problem, though.

My first $10$-second thought was that for every $n \equiv 1 \pmod{3}$, it would be impossible for the condition to be satisfied. This hypothesis seemed convincing since the case $n = 4$ is trivially true.

However, when I tried proving it, it came as no surprise that my efforts were unfruitful. I explored the case $n = 7$ to see what restrictions I would encounter that would prevent such a construction. To my surprise, a construction for $n = 7$ was possible, and  it convinced me divisibility by $3$ was a red herring, with the real obstruction being **Parity**.

$$
\begin{matrix}
\{1,2,3\}\\\\
\{1,4,5\}\\\\
\{1,6,7\}\\\\
\{2,4,6\}\\\\
\{2,5,7\}\\\\
\{3,4,7\}\\\\
\{3,5,6\}
\end{matrix}
$$

At this point, I asked a critical question that I believe finishes the problem: why does it work for $n = 7$ but not for $n = 4$?

If you shift your perspective and consider an individual soldier $a$, you realize that for the condition to be satisfied, $a$ must be the third member in tripples formed by adding $a$ to  all the possible pairs that can be formed with the remaining $n - 1$ soldiers i.e if $a$ is excluded. Consequently, if $n \equiv 0 \pmod{2}$, then $n-1$ is odd, so it is impossible to partition those soldiers into pairs. Therefore, no such construction can exist.
