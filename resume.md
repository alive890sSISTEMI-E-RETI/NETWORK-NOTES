#layer 2 o ripasso

pdu=frame

componenti -> router = interfaccia tra lan e internet
                questo componente triene un piede inn una rete e l altro nell'altro infatti ha due porte

direct delivery: MAC solo layer 2 (pin ip? traduzione da chiedere) e si utilizzano gli switch come intermediary device

# layer 3

pdu=pacchetto

connectionless best effort mesia indepensent

si gesisce la connessione tra sue LAN  -> ufficio postale

ip (end bit a bit) subnet = indirizzo di rete
se si eseguisse l'opearazione su due ip differenti si puo confrontare se sono uguali
in questo caso si possono paròate dirattamente

se nono e cosi allora visogna utilozzare il postino
a livello 3 si da effettivamente lìip completo. a livello due 


# layer 3

ip è l'indirizzo caratteristico del layer ed è gerarchico

proprietà: connectionless, universal addressing, best effort, routed protocol 
connectionless: ogni pacchetto viaggia indipendente
best effort: "io faccio il mio: se va male va..." il protocollo manda il pacchetto ma NON è lui a occuparsi di GARANTIRE 
la ricezione del pacchetto.
media independent: non imporata di quale mezzo trasmissivo si tratta "se decidiamo di andare al mare non tutti verremmo con la stessa macchina uno dietro l'altro, uno verrà in moto l'altro in pulman etch..."

tra il protocollo di layer 3 e 2 c'è un livello di interfaccia: LLC

ping indirizzo
if (indrizzo è nella mia lan) 
{
  dirct delivery
  il mio pc manda il suo mac nel prossimo pacchetto
}
else
{
  remote delivery
  si chiede di uscire al GATEWAY, router
}

quindi il giro è: ip esterno -> gateway mac con ip esterno -> ip esterno=ipGateway nope-> lo lancia su internet

ARP protocollo di livello 3 che funziona nel livello locale. Ip lavore l'affuori si occupa di instradare il pacchetto 
