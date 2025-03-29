grifinoria = 0
corvinal = 0
lufa_lufa = 0
sonserina = 0
print("Q1 Do you like Dawn or Dusk?")
print(" 1) Dawn")
print(" 2) Dusk")

answer = int(input("enter your answer (1-2): "))

if answer == 1:
  grifinoria += 1
  corvinal += 1
  print("Grifinória and Corvinal earn +1 point.")
elif answer == 2:
  lufa_lufa += 1
  sonserina += 1
  print("Lufa-Lufa and Sonserina earn +1 point.")
else:
  print("error! wrong entry.")

print("Q2) when i'm dead, i want people to remember me as:")
print("1) The Good")
print("2) The Great")
print("3) The Wise")
print("4) The Bold")

answer = int(input("enter your anwers (1-4): "))

if answer == 1:
  lufa_lufa += 2
  print("Lufa-Lufa earn +2 points.")
elif answer == 2:
  sonserina += 2
  print("Sonserina earn +2 points.")
elif answer == 3: 
  corvinal += 2 
  print("Corvinal earn +2 points.")
elif answer == 4:
  grifinoria += 2
  print("Grifinória earn +2 points.")
else:
  print("error! wrong entry.")

print("Q3) which kind of instrument most pleases your ear?")
print("1) The violin")
print("2) The trumpet")
print("3) The piano")
print("4) The drum")

answer = int(input("enter your answer (1-4): "))

if answer == 1:
    soserina += 4
    print("Sonserina earn +4 points.")
elif answer == 2:
    lufa_lufa += 4
    print("Lufa-Lufa earn +4 points.")
elif answer == 3:
    corvinal += 4
    print("Corvinal earn +4 points.")
elif answer == 4:
    grifinoria += 4
    print(" Grifinória earn +4 points.")
else:
    print("error! wrong entry.")

#exibir pontuação
print("\npontuação Final:")
print(f"Grifinória: {grifinoria} points.")
print(f"Sonserina: {sonserina} points.")
print(f"Lufa-Lufa: {lufa_lufa} points.")
print(f"Corvinal: {corvinal} points.")

#determinar a casa vencedora
casas= {
  "Grifinória": grifinoria,
  "Sonserina": sonserina,
  "Lufa-Lufa": lufa_lufa,
  "Corvinal": corvinal
}
casa_vencedora = max (casas, key=casas.get)
print(f"\nA casa que mais combina com você é: {casa_vencedora}. ")
