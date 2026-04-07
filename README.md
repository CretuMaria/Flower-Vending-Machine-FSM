# Flower-Vending-Machine-FSM
Descrierea Proiectului
Acest proiect reprezinta implementarea hardware a unui automat pentru vanzarea de flori (Flower Vending Machine), dezvoltat in limbajul de descriere hardware Verilog. Proiectul a fost realizat in mediul de dezvoltare Xilinx Vivado si demonstreaza conceptele de baza ale proiectarii logicii digitale, fiind dezvoltat in cadrul materiei "Sisteme cu Componente Integrate Digitale".

Concepte si Arhitectura
La baza functionarii acestui automat sta o Masina cu Stari Finite (FSM - Finite State Machine). Arhitectura sistemului asigura trecerea corecta si sigura prin diversele etape ale tranzactiei: starea de asteptare (IDLE), acumularea banilor inserati, verificarea balantei, eliberarea produsului si returnarea restului.

Functionalitati principale:
Sistem de introducere a banilor: Modulul accepta diferite tipuri de bancnote/monede (de ex. semnale distincte pentru 1, 5 sau 10 unitati/lei) si tine o evidenta interna a sumei acumulate.

Selectia produsului: Sistemul permite alegerea produsului dorit (buchetul de flori) si compara automat pretul acestuia cu suma introdusa de utilizator.

Eliberarea produsului (Dispense): In momentul in care suma acumulata este mai mare sau egala cu pretul florilor, sistemul activeaza semnalul de eliberare a produsului.

Calcularea si eliberarea restului: Logica interna calculeaza diferenta dintre suma introdusa si pretul produsului, trecand intr-o stare dedicata pentru returnarea restului catre utilizator.

Functionalitate de Reset: Dispune de un semnal de resetare globala (asincron/sincron) pentru a aduce masina la starea ei initiala, in cazul in care tranzactia este anulata.
