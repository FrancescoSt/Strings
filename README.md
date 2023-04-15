# Strings

## Descrizione programma
Programma c# per lo studio delle stringhe. Per creare questo file per la manipolazione delle stringhe non si sono usati le seguenti classi: ToUpper(), ToLower(), Count(), Lenght(), Replace(), IsLetter(), IsNumber(), infatti all'interno del programma tutte le classi sono state scritte manualmente.

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
  HSUHDUSHUSD

## Classi Manuali

ToUpper()

IsLetter()

IsDigit()

Lenght()


