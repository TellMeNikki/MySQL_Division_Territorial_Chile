# MySQL_Division_Territorial_Chile
SQL: Base de Datos con regiones,provincias y comunas de Chile, actualizado a nov.2022

### <h4>Script</h4>
el script consta de 2 parte:
<ul>
  <li>Creación de Base de Datos DB_DIVISION_TERRITORIAL_CHILE y respectivas Tablas Region,Provincia y Comuna</li>
  <li>Poblar Base de Datos desde SQL</li>
</ul>

Alternativamente se puede poblar la Base de Datos, importando desde archivos .CSV, para aquello reemplazar el script por el siguiente:

```
USE DB_DIVISION_TERRITORIAL_CHILE;
LOAD DATA
LOCAL INFILE '..\nombre_fichero.csv'
INTO TABLE 'NOMBRE_TABLA'
FIELDS TERMINATED BY ';'
LINES TERMINATED BY '\n'
CHARACTER SET  'utf8'
IGNORE 1 LINES;
```

Dónde 
  <ul>
    <li> nombre_fichero.csv ES comunas.csv,  provincias.csv ó regiones.csv </li>
    <li> NOMBRE_TABLA  ES Comuna, Provincia ó Region </li>
  </ul>
