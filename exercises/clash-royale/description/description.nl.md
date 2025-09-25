In het spel Clash Royale stel je een deck samen van verschillende kaarten, waarmee je tegen andere spelers strijdt. Soms wil je kaarten toevoegen of verwijderen om je deck te verbeteren. In deze oefening leer je hoe je een lijst van kaarten (je deck) automatisch kunt aanpassen op basis van een aantal veranderingen.

<img src="https://static0.gamerantimages.com/wordpress/wp-content/uploads/2025/02/clash-royale-electro-wizard-deck-1.jpg?q=49&fit=crop&w=825&dpr=2" width="200" height="100">

Schrijf een functie `verander_deck` die drie lijsten als argumenten krijgt:

1. `huidige_deck`: de huidige kaarten in het deck.
2. `deck_veranderingen`: de kaarten die toegevoegd of verwijderd moeten worden.
3. `voeg_toe`: een lijst met 0 of 1. 

Voor elke index in `voeg_toe` geldt:
- Staat er een 1, voeg dan de kaart op dezelfde index uit `deck_veranderingen` toe aan het deck.
- Staat er een 0, verwijder dan die kaart uit het deck.

Zorg ervoor dat de functie het aangepaste deck teruggeeft.

### Voorbeelden

```python
# Voorbeeld 1
huidige_deck = ["ridder", "boogschutter", "kanon"]
deck_veranderingen = ["kanon", "prinses", "ridder"]
voeg_toe = [0, 1, 0]
# "kanon" wordt verwijderd, "prinses" wordt toegevoegd, "ridder" wordt verwijderd
# Resultaat: ["boogschutter", "prinses"]

# Voorbeeld 2
huidige_deck = ["vuurgeest", "ijsgolem"]
deck_veranderingen = ["vuurgeest", "ijsgolem"]
voeg_toe = [0, 0]
# Beide kaarten worden verwijderd
# Resultaat: []

# Voorbeeld 3
huidige_deck = []
deck_veranderingen = ["tovenaar"]
voeg_toe = [1]
# "tovenaar" wordt toegevoegd
# Resultaat: ["tovenaar"]
```