# design-liferay-theme

Creazione di un tema per Liferay basato su "User Interface design guidelines".

## Getting Started

Il tema è stato realizzato per essere utilizzato sulla versione "Liferay Portal 6.2 CE GA6" in bundle con Tomcat-7.0.62. All'interno del tema sono presenti alcune portlet embeddate: la portlet della lingua, un form che si aggancia alla portlet della ricerca, la navigazione orizzontale (verticale nella modalità responsive). A titolo di esempio è stato riportato nell'header e nel footer tutto il contenuto presente nelle pagine di esempio contenute all'interno del Web Toolkit. Inoltre viene allegato una pagina html, con il cui codice è possibile creare un articolo web all'interno della piattaforma e pubblicarlo su una pagina.

### Prerequisites

Liferay Portal 6.2 CE GA6 bundle Tomcat-7.0.62
Maven

### Installing
Installazione tramite deploy nella relativa cartella sotto Liferay:

	Scaricare il progetto e lanciare il build tramite Maven.
	Copiare il war generato all'interno della cartella di DEPLOY presente nella installazione di Liferay.
	Una volta termminata l'installazione, loggarsi su Liferay e associare il tema alle pagine.
	

### TODO

All'interno del tema sono stati inseriti alcuni file contenuti all'interno del web toolkit: tra questi il file "Build.css". La presenza di alcune regole e attributi ha provocato errori dovuti alla compilazione con il SASS oltre a conflitti con i file css nativi di Liferay: per questo motivo, in fase di creazione si è scelto come "Parent theme" la versione "_unstyled", per limitare i conflitti. Il file Build.css è stato inserito tramite un link esterno (https://rawgit.com/italia/design-web-toolkit/gh-pages/design-web-toolkit/build/build.css). Si dovrà far coesistere i file nativi con quelli presenti nel web toolkit, conservando lo stile degli elementi nativi di Liferay, come Dockbar, controlli sulle portlet, ecc...


## Authors

* **Salvatore Costa** - *Initial work* - [tore72](https://github.com/tore72)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details