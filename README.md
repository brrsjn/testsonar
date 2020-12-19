Pasos para ejecutar el SonarQube
1. Descargarlo
    - Bajar SonarQube: https://www.sonarqube.org/downloads/
    - Bajar sonar-scanner: https://docs.sonarqube.org/latest/analysis/scan/sonarscanner/
2. Descomprimir
3. En el sonarqube-scanner se deben descomentar las propiedades(archivo en conf)
4. Crear un sonar-project.properties
    # required metdata
    sonar.projectKey=<preferrable_node_app_name>
    sonar.projectVersion=<version>
    sonar.sourceEncoding=<source code encoding>

    # path to srouce directories
    sonar.sources=<your_node_app_folder_name>

    # excludes
    sonar.exclusions=<files or folder which you want to exclude>

    # coverage reporting
    sonar.javascript.lcov.reportPaths=<code coverage location>

5. Añadir el path de la carpeta bin del scanner 
6. Correr el sonarqube server
7. iniciar proyecto, ejecutar codigo que trae consigo el token en la carpeta del directorio
