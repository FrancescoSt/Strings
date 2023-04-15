# Strings

## Descrizione programma
Programma c# per lo studio delle stringhe. Per creare questo file per la manipolazione delle stringhe non si sono usati le seguenti classi: ToUpper(), ToLower(), Count(), Lenght(), Replace(), IsLetter(), IsNumber(), infatti all'interno del programma tutte le classi sono state scritte manualmente. L'utente all'uall'inizio inserisce una stringa o una frase, e poi il programma va a fare vai test sulla manipolazione delle stringhe, tra cui le seguenti funzionalità: Maiuscola, Minuscola, Alfabetico, Alfanumerico, Numeri Lettere, Reverse.

## Funzionalità

* Maiuscola
```
  string Maiuscola(string s)
  {
  char[] caratteri = s.ToCharArray();
  
  for(int x=0; x<Lunghezza; x++)
  caratteri[x] = ToUpper();
    
  return new string(caratteri);
  }
```
Descrizione: Il metodo "Maiuscola" serve a far diventare la prima lettera di una stringa inserita dall'utente Maiuscola.
* Minuscola
```
  string Minuscolo(string s)
  {
  char[] caratteri = s.ToCharArray();
        
  for (int x = 0; x < Lunghezza(caratteri); x++)
  caratteri[x] = ToLower(caratteri[x]);

  return new string(caratteri);
  }
```
Descrizione: Il metodo "Minuscola" serve a far diventare la prima lettera di una stringa inserita dall'utente Minuscola.
* Reverse
```
 string Reverse(string s)
 {
 int len = Lunghezza(caratteri);
 char[] caratteri = s.ToCharArray();
 char[] tmp;
 for (int idx = 0; idx < len; idx++)
 {
 tmp = caratteri[idx];
 caratteri[idx] = caratteri[len];
 caratteri[len] = tmp;
 len--;
 }
 }
```
Descrizione: Il metodo "Reverse" serve a far invertire la stringa inserita dall'utente.
* Numero Lettere
```
  int NumeroLettere(string s)
	{
	int len = Lunghezza(caratteri);
	char[] caratteri = s.ToCharArray();
	int n;
	for(int idx=0; idx<len, idx++)
  {
	if (IsLetter(caratteri[idx]){

	n = n + 1;
	}
	}
	return n;
	}
```
Descrizione: Il metodo "Numero Lettere" serve per far capire all'utente il numero di lettere, dii una stringa inserita dall'utente.
* Se contiene caratteri alfabetici
```
  bool Alfabetico(string s)
	{
	char[] caratteri = s.ToCharArray();
	for(int i = 0; i<Lunghezza; i++)
	{
  if ((caratteri[i] >= 'a') && (caratteri[i] <= 'z') ||
  ((caratteri[i] >= 'A') && (caratteri[i] <= 'Z')
  {
	return true;
	}
	}
```
Descrizione: Il metodo Alfabetico rileva quanti caratteri alfabetici ci sono in una stringa che è stata inserita dall'utente.
*Se contiene solo caratteri alfanumerici
```
  bool Alfanumerico(string s)
	{
	char[]caratteri= s.ToCharArray();
  for (int i = 0; i < Lunghezza; i++)
		
  if(!((caratteri[i] >= 'a') && (caratteri[i] <= 'z') ||
  ((caratteri[i] >= 'A') && (caratteri[i] <= 'Z') ||
	(caratteri[i] >= '0') && (caratteri[i] <= '9')))
	{
	return false;
	}
  }
```
Descrizione: Il metodo Alfanumerico rileva quanti caratteri alfanumerici ci sono all'interno di una stringa inserita dall'utente.
## Classi Manuali

* ToUpper()
```
  char ToUpper(char c)
  {
  if( c >=  'a' && c <= 'z' )
  {
  int a = (int)c & 0xDF;
  return (char)a;
  }
  return c;
    }
```
Descrizione: questa classe serve per far diventare la prima lettera della stringa, Maiuscola.
* ToLower()
```
  char ToLower(char c)
  {
  if(c >= 'A' && c<= 'Z' )
  {
  int a = (int)c & 0xDF;
  return (char)a;

  }
  return c;
  }
```
Descrizione: questa classe serve per far diventare la prima lettera della stringa, Minuscola.
* IsLetter()
```
bool IsLetter(char c)
{
if (c >= 'A' && c <= 'Z')
{
int a = (int)c & 0xDF;
return (char)a;

}
return c;
}
```
Descrizione: Questa classe serve per capire quante lettere è formata una stringa.
* Lenght()
```
int Lunghezza(string comecavolomipare)
{
char[] caratteri = comecavolotipare.ToCharArray();
int retVal = 0;

foreach (char carattere in caratteri)
retVal++;

return retVal;
}
```
Descrizione: QUesta classe serve per capire la lunghezza della stringa, ovvero tutti i caratteri.
