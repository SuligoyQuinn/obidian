# 1
$p\oplus q\implies \neg r$
# 2
$r\implies p\lor q$
# 3
## a

| $a$   | $b$   | $a\underline{◼}b$ |
| ----- | ----- | ----------------- |
| True  | True  | True              |
| True  | False | True              |
| False | True  | False             |
| False | False | True              |

## b
$a\lor \neg b$
## c

| $a$   | $b$   | $b\underline{◼}a$ | $a\underline{◼}(b\underline{◼}a)$ |
| ----- | ----- | ----------------- | --------------------------------- |
| True  | True  | True              | True                              |
| True  | False | False             | True                              |
| False | True  | True              | False                             |
| False | False | True              | False                             |
