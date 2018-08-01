This repository contains the source code for generating the website published at http://vocab.linkeddata.es/datosabiertos

If you want to add a new vocabulary to the site you only need to include its URI in the Vocabularies CSV

Main developers: María Poveda and Daniel Garijo 

Other contributors: Miguel Angel García, Victor Rodríguez Doncel

Usage: java-jar vocab.jar -i input CSV file path [-o outputDirectoryPath]

If the -o flag is not inserted, a folder called site_+actualdate will be created.


A mezclar con la siguiente documentación:

En este repositorio se mantienen los vocabularios que se publican en http://vocab.linkeddata.es/datosabiertos

A continuación se describen los pasos para añadir un nuevo vocabulario:

A) Si tienes permisos de escritura sobre este repositorio

A.1) Añade una línea nueva al fichero Vocabularies.csv, con el formato: URI;{list of domains, comma separated}

A.2) Haz un commit en la master branch

B) Si no tienes permisos de escritura sobre este repositorio

B.1) Fork this repository

B.2) Add a new line to the Vocabularies.csv file with the format: URI;{list of domains, comma separated}

B.3) Commit it to the master branch and make a pull request when you are happy with it

B.3) Wait for any of the persons with write or admin permissions to accept it

Check the gh-page branch (e.g. http://opencitydata.github.io/vocabUpdates/site) to check whether the new site is ok or not before making the pull request to master (so that it is updated in vocab.linkeddata.es/datosabiertos)

