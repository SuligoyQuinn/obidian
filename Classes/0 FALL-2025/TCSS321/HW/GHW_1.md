Quinn Suligoy, Nicholas Cortes, Eli Labrador, Tristen Rodriguez

| $a$ | $b$ | $a\lor b$ | $a\underline{◼}b$ | $a\underline{◼}(a\underline{◼}b)$ |
| --- | --- | --------- | ----------------- | --------------------------------- |
| T   | T   | T         | T                 | T                                 |
| T   | F   | T         | T                 | T                                 |
| F   | T   | T         | F                 | T                                 |
| F   | F   | F         | T                 | F                                 |

We will define the squand operator "$a\underline{◼}b$" as equivalent to the proposition $a\lor \neg b$. From the proposition $a\lor b$ we can expand to $(a\lor b)\land T$ or $(a\lor b)\land(a\lor \neg a)$. Then using the distributive property we can pull the $a$ element out $a\lor(\neg a\land b)$. Then using DeMorgan's law we get $a\lor \neg(a\lor \neg b)$. Plugging in the squand identity we first get $a\lor \neg(a\underline{◼}b)$ and then $a\underline{◼}(a\underline{◼}b)$.