# **Spring framework**


![alt text](http://assets.spring.io/drupal/files/Logo_Spring_258x151.png "Logo Spring")


**L'Spring framework** (abreviant, Spring), és un marc de treball de codi obert per la plataforma _Java_. La primera versió va ser escrita per Rod Johnson, que inicialment va llençar el producte juntament amb el llibre One-on-One _Java_ EE Design and Development. També hi ha un port disponible per la plataforma .NET, Spring.NET.

El marc de treball va ser inicialment llençat al juny de 2003 sota la llicència Apache 2.0. La primera versió major 1.0 va ser distribuïda el març de 2004, amb llançaments addicionals el setembre de 2004 i març de 2005. Encara que **L'Spring framework** no força cap model de programació, ha esdevingut amplament popular dintre de la comunitat _Java_ primerament com una alternativa que desplaçaria el model Enterprise _Java_. Per disseny aquest entorn ofereix una gran llibertat als desenvolupadors de _Java_ i a més proveeix solucions fàcils i ben documentades per pràctiques habituals en la indústria.

Mentre les funcionalitats del nucli de l'entorn són usables en una aplicació _Java_ hi ha diferents extensions i millores per construir aplicacions web damunt d'una plataforma _Java_ EE. Gràcies a això, Spring ha aconseguit una gran popularitat i és reconegut pels fabricants com un entorn estratègicament important.

- Funcionalitats clau
- Introducció a Spring Framework
- Codi



## Funcionalitats clau


- Gestió de la configuració basada en ```JavaBeans```, aplicant-hi principis d'Inversió de Control, més específicament usant la tècnica d'Injecció de Dependència. Això ajuda a reduir les dependències de components, en implementacions específiques, sobre altres components.

- Una factoria de _Beans_ central, que és usada globalment.
- Capa genèrica d'abstracció per la gestió de transaccions de la base de dades.
- Estratègies preincorporades per la **JTA** i un sol DataSource de JDBC. Això elimina la dependència en un entorn _Java_   EE pel suport a les transaccions
- Integració amb entorns de persistència com **Hibernate, JDO, iBatis i db4o**.
- Entorn d'aplicació web _MVC_, construït al nucli de la funcionalitat de Spring. suportant moltes tecnologies per       generar vistes, incloent-hi **JSP, FreeMaker, Velocity, Tiles, iText i POI**.
- Entorn extensiu de ```programació orientada a aspectes``` per proveir serveis, com ara gestió de les transaccions. Amb a   això es millora la modularitat dels sistemes.


### Introducció a Spring Framework

**L'Spring framework** pot ser considerat com una col·lecció d'entorns més petits, o entorns dintre d'entorns. La majoria d'aquests estan dissenyats per treballar independentment uns dels altres, tot i que se suposa que junts, milloren les funcionalitats. Aquests mòduls estan dividits en blocs de construcció típics d'aplicacions complexes:

- **Contenidor d'Inversió de Control : configuració de components d'aplicació i gestió del cicle de vida d'objectes _Java_
- Entorn de Programació orientada a aspectes ([AOP](https://ca.wikipedia.org/wiki/Programaci%C3%B3_orientada_a_aspectes)):
- **Entorn d'accés a les dades**: treballant amb sistemes de gestió de bases de dades relacionals, sobre la plataforma _Java_ utilitzant [JDBC](https://ca.wikipedia.org/wiki/Java_Database_Connectivity) i eines de [mapeig objecte](https://ca.wikipedia.org/wiki/Mapatge_d%27objectes_relacional) - relacional ([JPA](https://ca.wikipedia.org/wiki/Java_Persistence_API), [Hibernate](https://ca.wikipedia.org/wiki/Hibernate) ...) aportant solucions a reptes tècnics que són reusables en una multitud d'entorns basats en _Java_.
- Entorn de gestió de transaccions: harmonització de diferents APIs de gestió de transaccions i orquestració de transaccions configuratives per objectes _Java_.
- **Entorn model-vista-controlador**: basat en HTTP i Servlet proveint moltes eines per la millora i la personalització.
- **Entorn d'accés remot**: importació i exportació d'objectes _Java_ a la manera de l'RPC (informàtica) configurable, sobre xarxes informàtiques que suporten protocols basats en [HTTP](https://ca.wikipedia.org/wiki/Protocol_de_transfer%C3%A8ncia_d%27hipertext), com ara [RMI](https://ca.wikipedia.org/wiki/Resson%C3%A0ncia_magn%C3%A8tica_nuclear), [CORBA](), i [serveis web](https://ca.wikipedia.org/wiki/Servei_web) ([REST](https://ca.wikipedia.org/wiki/REST)).
- **Entorn d'autenticació i personalització**: orquestració configurativa d'autenticació i processos d'autorització que suporten molts estàndards de la indústria, protocols, eines i pràctiques via el subprojecte Acegi security framework.
- **Entorn de missatgeria**: registre configurable d'objectes que reben missatges per la consumpció transparent de missatges des de cues de missatges via JMS, millora d'enviament de missatges sobre APIs JMS estàndards. Suport pel protocol AMQP (RabbitMQ, Kafka Broker...).
- **Entorn de testeig**: suporta classes per la creació d'unitats de testeig i proves d'integració.


## Codi

 ```java
 // Hola.java
import java.io.IOException;
public class Hola {
    public static void main(String[] args)throws IOException {
        System.out.println("Hola, món!"); 
    }
}
 ```



[Referencia per fer el markdown](https://ca.wikipedia.org/wiki/Spring_framework#M%C3%B2duls_de_l'Spring_Framework)






