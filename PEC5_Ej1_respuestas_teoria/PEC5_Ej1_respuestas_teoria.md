a) ¿Cuáles son las principales diferencias entre formularios dirigidos por template
y formularios reactivos?

Els formularis dirigits per plantilles utilitzen FormsModule, són asíncrons i la major part de la interacció es produeix en la plantilla. Mentres que els formularis reactius, utilitzen ReactiveFormsModule, són sincrònics i la major part de la interacció es produeix en el component.

b) ¿Qué son, para qué sirven y cómo se utilizan las directivas ngModel y 
ngModelChange?

Són etiquetes que el FormsModule te la capacitat d'utilitzar, serveixen per permetre el binding en dos direccions amb Angular i per tant, per simplicar l'ús dels formularis. 
Exemple: tenim un atribut del formulari per posar el nom del stock, dons amb el ngModel i el ngModelChange, relacionem aquests input amb l'atribut name de l'objecte stock.
<input type="text"
    placeholder="Name"
    name="Name"
    [ngModel]="stock.name"
    (ngModelChange)="stock.name=$event">

c) ¿Qué son, cuáles son y para qué sirven los estados en los formularios dirigidos 
por templates?

Els estats ens permeten tindre coneixement sobre l'estat del control del formulari, sobre si l'usuari l'ha visitat, si l'ha canviat o bé si ha estat vàlid. Ho sabem segons la classe CSS que tingui l'element.
Els estats són Visitat, Canviat i Vàlid.

d) ¿Qué ventajas aportan los FormGroup en la composición de formularios?

Ens aporta una millor organització i administració dels elements d'un formulari, com per exemple, tindre agrupat en un FormGroup els elements que estan relacionats, de tal manera que si un element ja no es vàlid, tot el grup no és vàlid.