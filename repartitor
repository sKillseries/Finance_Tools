#!/usr/bin/python3

def calculer_proportion(salaire, somme_totale):
    proportion = (salaire / somme_totale)
    return proportion

def main():
    nombre_personnes = 2  # Le foyer est constitué de 2 personnes
    salaires = []

    for i in range(nombre_personnes):
        salaire = float(input(f"Entrez le salaire de la personne {i+1} : "))
        salaires.append(salaire)

    somme_totale_revenus = sum(salaires)

    charges_foyer = float(input("Entrez le montant total des charges du foyer : "))

    proportions = [calculer_proportion(salaire, somme_totale_revenus) for salaire in salaires]

    charges_par_personne = [charges_foyer * proportion for proportion in proportions]

    print("\nRépartition des charges du foyer :")
    for i, montant in enumerate(charges_par_personne):
        print(f"Personne {i+1} : {montant:.2f}€")

if __name__ == "__main__":
    main()
