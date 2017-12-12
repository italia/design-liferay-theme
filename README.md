> **ATTENZIONE:**
> Questo repository contiene software in versione sperimentale, e non è ancora pronto per un utilizzo in produzione. Verificare lo stato di avanzamento del progetto nella sezione [TODO](#todo) oppure consultando le [issue aperte](https://github.com/italia/design-liferay-theme/issues).

[![Build Status](https://travis-ci.org/italia/design-liferay-theme.svg?branch=master)](https://travis-ci.org/italia/design-liferay-theme)
[![Join the #design-liferay-theme channel](https://img.shields.io/badge/Slack%20channel-%23design--liferay--theme-blue.svg)](https://developersitalia.slack.com/messages/C8CR7RFTQ)
[![Get invited](https://slack.developers.italia.it/badge.svg)](https://slack.developers.italia.it/)

# design-liferay-theme

Creazione di un tema per Liferay basato su "User Interface design guidelines".

## Getting Started

Il tema è stato realizzato per essere utilizzato sulla versione "Liferay Portal 6.2 CE GA6" in bundle con Tomcat-7.0.62. All'interno del tema sono presenti alcune portlet embeddate: la portlet della lingua, un form che si aggancia alla portlet della ricerca, la navigazione orizzontale (verticale nella modalità responsive). A titolo di esempio è stato riportato nell'header e nel footer tutto il contenuto presente nelle pagine di esempio contenute all'interno del Web Toolkit. Inoltre viene allegato una pagina html, con il cui codice è possibile creare un articolo web all'interno della piattaforma e pubblicarlo su una pagina.

### Prerequisites

 * [Liferay Portal 6.2 CE GA6 bundle Tomcat-7.0.62](https://sourceforge.net/projects/lportal/files/Liferay%20Portal/6.2.5%20GA6/)
 * [Maven](https://maven.apache.org/download.cgi)

### Installing
Installazione tramite deploy nella relativa cartella sotto Liferay:
 
 * Scaricare il progetto e lanciare il build tramite Maven utilizzando il comando: `mvn clean install -Dmaven.test.skip=true`.
 * Copiare il war generato all'interno della cartella di DEPLOY presente nell'installazione di Liferay.
 * Una volta termminata l'installazione, loggarsi su Liferay e associare il tema alle pagine.


### TODO

 * All'interno del tema sono stati inseriti alcuni file contenuti all'interno del web toolkit: tra questi il file "Build.css". La presenza di alcune regole e attributi ha provocato errori dovuti alla compilazione con il SASS oltre a conflitti con i file css nativi di Liferay: per questo motivo, in fase di creazione si è scelto come "Parent theme" la versione "_unstyled", per limitare i conflitti. Il file Build.css è stato inserito tramite un link esterno (https://rawgit.com/italia/design-web-toolkit/gh-pages/design-web-toolkit/build/build.css).
 * Non è ancora completata inoltre la lavorazione per far coesistere i file nativi con quelli presenti nel web toolkit, conservando lo stile degli elementi nativi di Liferay, come Dockbar, controlli sulle portlet, ecc...


## Authors

* **Salvatore Costa** - *Initial work* - [tore72](https://github.com/tore72)

## License

This project is licensed under the BSD-3-Clause License - see the [LICENSE](LICENSE) file for details
