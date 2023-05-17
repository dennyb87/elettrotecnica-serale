# Risoluzione per contraddizione  

> picture here

Talvolta puo' succedere che non sia immediatamente ovvio se il diodo e' in conduzione oppure no, e' possibile allora procedere ipotizzando una delle due situazioni. Ipotizziamo per esempio che sia in conduzione. Se il diodo e' in conduzione ci aspettiamo che la seconda legge di Kirchhoff sia in accordo con la nostra ipotesi.  

$V_{FC} + V_{CB} + V_{BA} + V_{AG} + V_{GF} = 0$  

$R_1I + V_D + R_2I + \cancel{E} - \cancel{E} = 0$  

$V_D = -R_1I-R_2I \implies -R_1I-R_2I \le 0$  

Se $V_D$ e' minore o uguale a zero allora siamo giunti ad una contraddizione, e la nostra ipotesi era falsa! Il diodo non e' in conduzione!
