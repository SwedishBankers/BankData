# Bank data Clearing och IBAN uppgifter för svenska banker

Sammanställning av data i maskinläsbart format från Bankgirot och Swedishbankers för validering och uträkning av clearingnummer och IBAN konto

## Data, updateringar och källor
Se [Readme i Data](Data)

## Avvikelser

### Nordea 3300, 3782
3782 används i praktiken inte, betalning via 3300 och 3782 går till samma konto. (Det förekommer att banker inte tillåter 3782)

### Handelsbanken 6000-6999
Alla konton i serien är unika, oavsett clearing. Konvertering från IBAN kan använda valfrit clearingnr.

### Swedbank 8000-8999
Swedbank hänvisar till https://www.swedbank.se/privat/betala-och-overfora/iban-och-bic.html och skriver att om kontot inte är giltigt där så är kontot ogiltigt. (Alternativ som är lättare att testa med: https://jsfiddle.net/mzwe8coh/2/)  
Texten i Bankgirots information kan ignoreras "I sällsynta fall förekommer dock Swedbanks kontonummer som inte alls är kontrollerbara med kontrollsiffra."

### Sparbanken Syd 9570-9579  
Använder endast 9570