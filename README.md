# Sääbotti

Sääbotti on Facebookin wit.ai-alustan avulla tehty botti. Se ymmärtää sille luonnollisella kielellä annettuja pyyntöjä kertoa sää. Merkittävä osa tämän botin toiminnallisuudesta luodaan käyttämällä wit.ai:n verkkosivua osoitteessa wit.ai. 
 
Botti on kirjoitettu python-kielellä ja se käyttää hyväkseen wit.ai:n lisäksi voikko-nimistä työkalua. Voikon avulla saadaan sovellus “ymmärtämään” suomenkieltä, sillä wit.ai:n suomenkielen tuki on vielä vaiheessa. Voikon asentaminen on haastavaa ja helpoiten sen saa ubuntu-käyttöjärjestelmän mukana. Python valittiin sääbotin ohjelmointikieleksi, sillä sen avulla on helpohko kommunikoida voikon kanssa libvoikko-kirjaston avulla.
 
Asennettuasi voikon ja tarvittavat python kirjastot (requests, libvoikko) laita allaolevat tiedostot samaan kansioon ja ja aja weather.py komennolla python3 weather.py.

## Vaatimukset

Ohjelman suorittaminen vaatii Python 3 -tulkin, Voikko-ohjelman ja PIP-pakettimanagerin.

## Asennus suomenkielisellä ubuntu-käyttöjärjestelmällä (jossa Voikko tulee sisäänrakennettuna)


1. Hae koodi `git clone https://github.com/Mikrobitti/6-17-saabotti.git` 
2. `pip install requests`
3. `apt-get install python-libvoikko`
4. Luo tili wit.ai:hin ja opeta bottisi. Asetukset sivulta löydät sovelluksesi palvelinavaimen.
5. Laita tarvittavat ympäristömuuttujat paikoilleen: `export WIT_SERVER_ACCESS_TOKEN=[oma palvelinavaimen]` ja `export FMI_API_KEY=[oma api-avaimesi ilmatieteenlaitoksen rajapintaan]`. Ilmatieteenlaitoksen rajapintaan saat tunnukset osoitteesta https://ilmatieteenlaitos.fi/rekisteroityminen-avoimen-datan-kayttajaksi


## Aja koodi komennolla

`python3 weather.py`
