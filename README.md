# Enapp Braindump Solutions

 <i style=float:right;>paiva dias</i> <br>

## REST & SOAP

Was ist REST?  
* (Kein Standard/Protokoll, eher Design Pattern)

Auf was baut REST auf?  
* (Bestehende Protokolle zB HTTP. Nichts neues erfunden. Bestehendes verwendet.)

Wie läuft eine REST-Trasaktion ab??  
* (Äh Zugriff per URI, auf einzelne Ressource über HTTP-Verben)

Was sind die 4 Grund HTTP-Verben?  
* (GET, POST, DELETE, PUT)

Was ist Impoponent?  
* (Mehrfachzugriff sollte Daten nicht verändern)

Bei welchen HTTP-Verb gibt es einen Sonderfall?  
* (Bei PUT - Beispiel mit Counter)

Wie ist SOAP aufgebaut?   
* (XML Dokument mit Envelope->Head und Body)

Wie funktioniert SOAP?  
* (Zugriff nur über eine einzelne URL. SOAP Server entscheided mit Hilfe des XML Bodys)

Unterschied zwischern SOAP und REST?  
* (Alle nötigen Informationen für Router, Firewall, etc stehen im Header. Gut für Caching).

Was sollen Router und Firewalls nie machen?  
* (Nie in den Payload der Daten reinschauen. WICHTIG Payload und nicht Content oder Data als Stichwort verwenden)

## Web-Tier

Wie implementieren Sie ein Servlet?  
* (Interface oder von GenericServlet/HTTPServelt erben)

Auszeichnen Zustände / LifeCycle von einem Servlet.  
* (init(), destroy(), service(), doGet(), ...)

MVC Pattern aufzeigen/-zeichnen und wie im Projekt verwendet.   
* (Model=Bean, View=JSF, Controller=Servlet)


## CDI & EJB

was für IoC Pattern gibt es
Class Loader, CDI


Beide Patterns von IoC zeichnen


Was bedeuten die Pfeile



Anatomie von Beans?   
* ein (nicht leeres) Set von Bean Typen   
* ein (nicht leeres) Set von Qualifiers   
* ein Scoope  
* Optional, ein Beam EL Name   
* Ein Set von Interceptor Bindings   
* Eine Bean Implementaion  
* kann eine Alternative* haben

Was ist ein Bean Typ?

Ein Bean Typ ist eine __user definierte Klasse__  
einem Typ der __client-visible ist.__

Session Beans & Message Driven Beans

Was für Scope Annotations gibt es?

* @RequestScoped  
* @SessionScoped  
* @ApplicationScoped  
* @ConversationScoped


welche Services bietet CDI an?
* verbesserter Lebenszyklus für stateful Objekte die an definierte Kontexte gebunden sind.  
* Typen sichere Dependency Injection 
* Objekt Interaktion via Event Notification Facillity 
* Ein verbesserter Ansatz um Interceptoren an Objekte zu binden. Verwendet wird ein neuer Interceptor, genannt Decorator um neuen Business Anforderungen zu genügen.  
* SPI um portierbare Extensions fuer den Kunden zu entwickeln.
