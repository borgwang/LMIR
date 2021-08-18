# LMIR

Pure Python implementations of the language models for information retrieval surveyed [here](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.94.8019&amp;rep=rep1&amp;type=pdf).

## score calculation
```
# Jelinek-Mercer
score(q, d) = -log(p(q|d))
p(q|d) = p(t_1|d) * p(t_2|d) * ... * p(t_k|d)
p(t_i|d) = (1 - lamb) * (TF(t_i, d) / LEN(d)) + lamb * (TF(t_i, C) / LEN(C))
```
