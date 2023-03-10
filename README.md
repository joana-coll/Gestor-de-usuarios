<!-- T脥TULO Y DESCRIPCI脫N -->
  <a name="ir-arriba"></a>
  # 馃捇 Gestor de usuarios

  Trabajo Pr谩ctico Final para el curso **Codo a Codo Java Spring Boot 2022**
  <div align="center">
    <table>
      <tr>
        <td>
        Consigna: API REST CRUD con Tests unitarios y de integraci贸n que contenga los temas vistos a lo largo de la cursada
        </td>
        <td>
          <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/PROYECTO.png" width="250px">
        </td>
      </tr>
    </table>
  </div>

<!-- 脥NDICE -->
  <a name="indice"></a>
  ## 馃搶 脥ndice
  <ol>
    <li><a href="#ir-arriba">T铆tulo y descripci贸n del proyecto</a></li>
    <li><a href="#indice">脥ndice</a></li>
    <li><a href="#tecnologias">Tecnolog铆as utilizadas</a></li>
    <li><a href="#instalacion">Instalaci贸n</a></li>
    <li><a href="#funcionalidad">Funcionalidad de la App</a>
      <ul>
        <li><a href="#crear-persona">Crear persona</a></li>
        <li><a href="#ver-todas-las-personas">Ver todas las personas</a></li>
        <li><a href="#ver-persona">Ver persona</a></li>
        <li><a href="#editar-persona">Editar persona</a></li>
        <li><a href="#borrar-persona">Borrar persona</a></li>
        <li><a href="#cantidad-de-personas-por-g茅nero">Cantidad de personas por g茅nero</a></li>
        <li><a href="#persona-de-mayor-edad">Persona de mayor edad</a></li>
        <li><a href="#persona-de-menor-edad">Persona de menor edad</a></li>
        <li><a href="#personas-por-provincia">Personas por provincia</a></li>
        <li><a href="#validaciones">Validaciones</a></li>
        <li><a href="#tests-unitarios-y-de-integraci贸n-con-coverage">Tests unitarios y de integraci贸n con Coverage</a></li>
      </ul>
    </li>
    <li><a href="#desarrollado">Desarrollado por...</a>
    <li><a href="#contacto">Contacto</a>
    <li><a href="#agradecimiento">Agradecimiento</a>
  </ol>

<!-- TECNOLOG脥AS UTILIZADAS -->
  <a name="tecnologias"></a>
  ## 鉁? Tecnolog铆as utilizadas
  <p align="center">
    <a href="https://www.java.com/" target="_blank">
      <img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=java&logoColor=white">
    </a>
    <a href="https://spring.io/" target="_blank">
      <img src="https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white">
    </a>
    <a href="https://maven.apache.org/" target="_blank">
      <img src="https://img.shields.io/badge/apache_maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white">
    </a>
    <a href="https://github.com/" target="_blank">
      <img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white">
    </a>
   </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>

<!-- INSTALACI脫N -->
  <a name="instalacion"></a>
  ## 馃敡 Instalaci贸n
  Si deseas correr la aplicaci贸n en un entorno local debes tener en cuenta lo siguiente: 
  1. Clona el repositorio utilizando GIT o descargando el archivo ZIP:

      `git clone https://github.com/joana-coll/Gestor-de-usuarios.git`
  
  2. El proyecto viene configurado para ejecutarse en el entorno de desarrollo y utilizar los endpoint. Si deseas probar los tests debes modificar el archivo `application.yml` y reemplazar `local` por `integration_test`
  
  3. Para probar los endpoint es recomendable utilizar Postman
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>
  
<!-- FUNCIONALIDAD DE LA APP -->
  <a name="funcionalidad"></a>
  ## 鈿欙笍 Funcionalidad de la App
  La aplicaci贸n es un CRUD de personas. Los atributos poseen validaciones y contiene tests unitarios y de integraci贸n. Adem谩s cuenta con los siguientes endpoints:
  <ul>
    <li>/persona/crear</li>
    <li>/persona/verTodos</li>
    <li>/persona/ver/{id}</li>
    <li>/persona/editar/{id}</li>
    <li>/persona/borrar/{id}</li>
    <li>/persona/porGenero</li>
    <li>/persona/mayor</li>
    <li>/persona/menor</li>
    <li>/persona/porProvincia/{provincia}</li>
  </ul>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>

### Crear persona
  `/persona/crear` agrega a una persona mediante un _RequestBody_ validando los datos de nombre, apellido, edad, g茅nero, dni y provincia
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/CREAR%20OK%201.png" width="600px">
  </p>
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/CREAR%20OK%202.png" width="450px">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/CREAR%20KO.png" width="450px">
  </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>

### Ver todas las personas
  `/persona/verTodos` muestra todas las personas
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/VER%20TODOS.gif" width="450px">
  </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>

### Ver persona
  `/persona/ver/{id}` muestra a una determinada persona por id mediante un _PathVarible_
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/VER%20POR%20ID%20OK.png" width="450px">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/VER%20POR%20ID%20KO.png" width="450px">
  </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>
  
### Editar persona
  `/persona/editar/{id}` edita a una persona mediante un _RequestBody_ enviando el id por _PathVariable_ 
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/EDITAR%20OK%201.png" width="600px">
  </p>
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/EDITAR%20OK%202.png" width="450px">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/EDITAR%20KO.png" width="450px">
  </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>
  
### Borrar persona
  `/persona/borrar/{id}` borra a una determinada persona por id mediante un _PathVariable_
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/BORRAR%20OK.png" width="450px">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/BORRAR%20KO.png" width="450px">
  </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>

### Cantidad de personas por g茅nero
  `/persona/porGenero` muestra la cantidad de personas masculinas y femeninas que hay
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/POR%20GENERO.png" width="600px">
  </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>
  
### Persona de mayor edad
  `/persona/mayor` muestra la persona de mayor edad
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/MAYOR.png" width="450px">
  </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>
  
### Persona de menor edad
  `/persona/menor` muestra la persona de menor edad
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/MENOR.png" width="450px">
  </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>
  
### Personas por provincia
  `/persona/porProvincia/{provincia}` muestra las personas que hay en una determinada provincia enviada mediante _PathVariable_
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/POR%20PROVINCIA.gif" width="450px">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/POR%20PROVINCIA%20KO.png" width="450px">
  </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>
  
### Validaciones
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/VALIDACION%20NOMBRE.png" width="500px">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/VALIDACION%20APELLIDO.png" width="500px">
  </p>
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/VALIDACION%20EDAD.png" width="300px">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/VALIDACION%20GENERO.png" width="300px">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/VALIDACION%20DNI.png" width="300px">
  </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>
  
### Tests unitarios y de integraci贸n con Coverage
  <p align="center">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/TEST%20CON%20MOCKITO.png" width="300px">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/INTEGRATION%20TEST.png" width="300px">
    <img src="https://github.com/jc-projects/CodoACodo_SpringBoot_TP_Final/blob/main/README/COVERAGE.png" width="450px">
  </p>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>
  
<!-- DESARROLLADO POR -->
  <a name="desarrollado"></a>
  ## 馃拋 Desarrollado por...
  * **Joana Coll** - [joana-coll](https://github.com/joana-coll)
  
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>
  
<!-- CONTACTO -->
  <a name="contacto"></a>
  ## 馃摡 Contacto
  Si deseas contactarte conmigo:
  <a href="https://ar.linkedin.com/in/joana-coll" target="_blank">
  <img src="https://raw.githubusercontent.com/joana-coll/joana-coll/1ce466f12c925e1e39ab93b44ff985f102c9aed8/icons/linkedin.svg" alt="Github" height="30" />
  </a>
  <a href="mailto:colljoana@gmail.com" target="_blank">
  <img src="https://raw.githubusercontent.com/joana-coll/joana-coll/1ce466f12c925e1e39ab93b44ff985f102c9aed8/icons/envelope-solid.svg" alt="Github" height="30" />
  </a>
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>

<!-- AGRADECIMIENTO -->
  <a name="agradecimiento"></a>
  ## 鉂わ笍 Agradecimiento
  Gracias por leer hasta aqu铆, espero que el proyecto te sea 煤til. No tiene Licencia pero podes usarlo como gustes mientras sigas fomentando el c贸digo libre y ayudando a otros pares. 
  
  隆Que tengas un lindo d铆a!
  
  Nana 鉁?
  <p align="right">(<a href="#ir-arriba">Ir arriba</a>)</p>
