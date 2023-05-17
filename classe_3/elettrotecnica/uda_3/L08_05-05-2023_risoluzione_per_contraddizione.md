# Risoluzione per contraddizione  

![proof_by_contradiction_in_circuit_analysis](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/9eae1726-73bd-4ad2-b1f0-ac20fc3eec84)  

Talvolta puo' succedere che lo stato del diodo non sia facilmente intuibile, e' possibile allora procedere ipotizzando una delle due situazioni. Ipotizziamo per esempio che sia in conduzione. Se il diodo e' in conduzione ci aspettiamo che la seconda legge di Kirchhoff sia in accordo con la nostra ipotesi, ovvero ci aspettiamo di trovare su $V_{D_1}$ una tensione di circa $0.7\ V$.  

$V_{FC} + V_{CB} + V_{BA} + V_{AG} + V_{GF} = 0$  

$R_2I + V_{D_1} + R_1I + \cancel{E_1} - \cancel{E_2} = 0$  

$V_{D_1} = -R_1I-R_2I  \le 0$  

Se $V_{D_1}$ e' minore o uguale a zero allora siamo giunti ad una contraddizione, e la nostra ipotesi era falsa! Il diodo non e' in conduzione!  
