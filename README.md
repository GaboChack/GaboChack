while True:
    P1 = float(input("Dime tú calificación de  primer periodo : "))
    P2 = float (input("Dime tú calificación de segundo perdido: "))
    P3= float (input( "Dime tú calificación de tercer perdiodo: "))
       
    Final =((P1+P2+P3)/3)
    print ("Tú calificación de los 3 periodos es: ",Final)
    if Final >= ( 9.5):
      print ("Exentaste")
      c = (Final*.40)
      c2 = (c+6)
      print ("Tú calificación final de los periodos ", c2)
      break 
    else:
     print("Te vas al semestral")
     S2 = (Final * .60)
     S3 = abs(S2  - 6)
     print ("necesitas sacar ",S3,"para tener el 6 final ")
     coeff = 0.40
     constant = S3
     def solve_equation(coeff, constant):
      solution = constant / coeff
      return solution
     solution = solve_equation(coeff, constant)
     print("Tienes que sacar en el examen " , solution)
     Semestral = float(input("dime tú calificación de semestral : "))
     S1 = (Semestral *.40)
     Final2 = (S1+S2)
     if Final2 >= (6 ):
         print("Pasámooooooos SUUUU")
         print ("NO te vas a extra")
         print("Tú calificación final es: ",Final2)
         break
     else :
        print ("Te vas al EXTRA")
        print("Tú calificación final es: ",Final2)
        break


