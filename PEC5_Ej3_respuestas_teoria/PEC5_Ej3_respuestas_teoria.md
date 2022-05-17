a) ¿Qué son, para qué sirven y cómo se utilizan FormControl, FormGroup y 
FormBuilder?

FormControl: es una classe que encapsula tota la informació relacionada amb un element input, on podem saber l'estat de validació d'aquest i afegir regles de validació.
FormGroup: en comptes d'utilitzar un FormControl per a cada input, podem agrupar els elements que estigen relacionats en un FormGroup, per a poder organizar i administrar aquests, i ens estalviem utilitzar tants FormControl.
FormBuilder: es la API auxiliar per crear formularis en Angular, proporciona accès directe per a crear les instàncies de FormControl, FormGroup o FormArray.

b) Busca en la página oficial de Angular (o utiliza un recurso de O’Reilly) en el que 
se especifiquen todos los validadores que incluye Angular para ser utilizados en 
los formularios reactivos. Construye una tabla de resumen de estos.

https://angular.io/api/forms/Validators

| Validators         | Descripció     |
|--------------|-----------| 
| min |  requereix que el valor sigui major o igual al número proporcionat  | 
| max |  requereix que el valor sigui menor o igual al número proporcionat  | 
| required |  requereix que el camp no sigui buit  | 
| requiredTrue  |  requereix que el valor sigui true, es sol utilitzar per als checkbox  |  
| email  |  requereix que el valor ha de pasar una prova de validació de correu electrònic  | 
| minLength  |  requereix que la longitud del valor sigui superior o igual al número proporcionat  | 
| maxLength  |  requereix que la longitud del valor sigui menor o igual al número proporcionat  | 
| pattern    |  requereix que el valor coincideixi amb un patró de regex  | 
| nullValidator |  no realitza cap operació  | 
| compose       |  composa diversos validadors en una única funció que retorni la unió dels mapes d'error individuals per al control proporcionat  | 
| composeAsync  |  composa diversos validadors asíncrons en una única funció que retorni la unió dels objectes d'error individuals per al control proporcionat  | 


c) ¿Qué son, cuáles son y para qué sirven los estados en los formularios reactivos?

Els estats ens permeten tindre coneixement sobre l'estat del control del formulari, sobre si l'usuari l'ha visitat, si l'ha canviat o bé si ha estat vàlid. Ho sabem segons la classe CSS que tingui l'element.
Els estats són Visitat, Canviat i Vàlid.