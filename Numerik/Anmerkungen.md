#Regula-falsi
Schnittpunkt von (a, f(a)) (b, f(b)) mit der Geraden {y = 0} sei (c, 0)

Ist sign(f(c)) = sign(f(a)), dann wird a im nächsten Iterationsschritt auf c gesetzt
Ist sign(f(c)) = sign(f(b)), dann wird b im nächsten Iterationsschritt auf c gesetzt

#Newtonverfahren
Schnittpunkt der Sekanten an der Stelle (x, f(x)) mit der Geraden {y = 0} sei (c, 0)

x wird im nächtsten Iterationsschritt auf c gesetzt

#Sekantenverfahren
Schnittpunkt der Geraden durch (xn, f(xn)) und (x[n+1], f(x[n+1])) mit der Geraden {y = 0} sei (c, 0)

xn wird im nächsten Iterationsschritt auf x[n+1] gesetzt, x[n+1] auf c

#Banachscher Fixpunktsatz
M metrischer Raum, also hat eine Distanz ziwschen zwei Elementen, die mit d berechnet wird
Kontraktionsabbildung φ: M -> M, die sich höchstens mit 0 <= λ < 1 ändert
φ hat einen Fixpunkt, i.e. φ(ξ) = ξ

x[n+1] := φ(xn) konvergiert gegen ξ

##Abschätzung der Distanz des n-ten Folgengliedes durch die Distanz der ersten beiden Folgenglieder
d(xn, ξ) ≤ (λ ^ n) * d(x0, x1) / (1 - λ)

##Abschätzung der Distanz des n-ten Folgengliedes durch die Distanz der letzten beiden Folgenglieder
d(xn, ξ) ≤ λ * d(x[n-1], xn) / (1 - λ)

#Iterationsabbildung:
Die Ergebnisse eines Schrittes werden als Ausgangswerte des jeweils nächsten Schrittes genommen.
Die Folge der Ergebnisse muss konvergieren..

#Konvergenzordnung:
##Linear
Lineare Konvergenzgeschwindigkeit, falls ein 0 < c < 1:
norm(x[k+1] - x) ≤ norm(xk - x) * c für alle k

##Ordnung p
Konvergenz der Ordnung p, falls auch ein p > 1:
norm(x[k+1] - x) ≤ norm(xk - x)^p * c für alle k