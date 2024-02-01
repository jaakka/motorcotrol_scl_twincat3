# moottoriohjaus scl twincat3

Moottorin ohjauskoodi 3-vaiheiselle moottorille jossa rele1 ja rele2 ovat moottorin päinvastaiset kytkennät eli
nämä eivät saa olla samaan aikaan päällä ja esim rele2 moottorille menee vaiheet eri järjestyksessä kuin rele1 , 3 eri toiminta tavalle. 

### Variables.scl #### Aloitus muuttujat
### Main.scl #### Aloitus muuttujat

Testausten mukaan koodia suoritetaan 60 kertaa sekunnissa mutta en ole vielä testannut logiikalla
että täsmääkö tämä aika joten sitä saattaa joutua nostamaan. 

1. toiminta tapa (Manuaaliajo)
   Painike1 käynistää moottorin.
   Painike2 käynistää moottorin toisinpäin.
   Painike3 pysäyttää moottorin.
   Moottorin ja ajastimen pitää olla pysähtynyt että voidaan painaa 1 tai 2.

2. toiminta tapa (Automaattiajo)
   Painike1 aloittaa automaatti ajon joka toimii vaiheittain ja
   tietyillä aikaväleillä. Painike3 pysäyttää automaattiajon ja moottorin.

3. toiminta tapa (Anturiajo)
   Painike1 aloittaa ajon ja kun anturi1 tai anturi2 reagoi,
   moottori vaihtaa tarvittaessa suuntaa.
   Painike3 pysäyttää anturivalvonnan ja moottorin.
