aceptadas = {"aa", "aabbaa", "cabacaba"}
rechazadas = {"a", "abc", "aaa"}
 
def evaluar_cadena(cadena):
    if cadena in aceptadas:
        return "Aceptada"
    elif cadena in rechazadas:
        return "Rechazada"
    else:
        return "No definida"
# Pruebas
cadenas = ["aa", "a", "aaa", "cabacaba", "abc", "aabbaa"]
for c in cadenas:
    print(c, "->", evaluar_cadena(c))
