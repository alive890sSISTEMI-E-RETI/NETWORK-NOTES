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

# layer 3
il livello 3 è un po' come il GPS
CARATTERISTICHE: 
* Connectionless: "non ci teniamo la manina", partenza e destinazione hanno più vie percorribili
* Best Effort: "se non arrivo almeno ci ho provato"
* Media Independence: il protocollo gira su qualunque mezzo di trasmissione

prima IP era adottato nelle WAN esclusivamente, poi anche nelle LAN(1996)ù
l'indirizzo IP è LOGICO e GERARCHICO

### PROTOCOLLO ARP


## indirizzi speciali
0.0.0.0/0 (uguale) vuol dire un indirizzo che MATCHA tutti gli indirizzi 
x.x.1.1/16 (variabile) indirizzo di BROADCAST
127.0.0.1 (uguale) loopback
x.x.0.0 (variabile) serve per identificare la sottorete (NON L'HO CAPITO)

internet vuol dire interconnessione di reti collegate remotamente collegate tramite protocollo ip  (=WAN GEOGRAFICA)


il passaggio sarebbe creare una INTRANET per avere accesso a INTERNET tramite questo GATEWAY


Indirizzamento DIRETTO vs INDIRETTO: nel primo di comunica solo con switch, nel secondo caso si scomoda lo switch
