<script>
import Competencias from "../../lib/paginas/componentes/competencias.svelte";
import Contenido from "../../lib/paginas/componentes/contenido.svelte";
import Salidas from "../../lib/paginas/componentes/salidas.svelte";
import MenuAside from "../../lib/paginas/menuAside.svelte";
import Accesotable from "../../lib/paginas/componentes/accesotable.svelte";

</script>

<main>

<!--MENU NAVEGADOR-->
    <MenuAside/>


<!--APARTADOS-->
<div class="encabezado">
    <h1>CURSO ESPECIALIZADO EN CIBERSEGURIDAD <br>
        <i class="fa fa-graduation-cap"></i>
    </h1>
</div>

<Competencias
    src= "src/images/paginas/ciberseguridad.jpg"
    competenciastext="La figura del especialista en Ciberseguridad se ha convertido en imprescindible en una sociedad en la que la presencia de delitos digitales es cada vez más común.
    Si estás pensando en dedicarte a la protección de la seguridad en la red, necesitarás una gran especialización y conocimientos avanzados en derecho e informática."
/>

<div class="card" id="salidas-profesionales">
    <h1 style="color: white" >SALIDAS PROFESIONALES</h1>
        <div class="salidas-box">
                    <Salidas
                        div ="div1"
                        carrera="Arquitecto de seguridad."
                        icon="fa-solid fa-folder-tree"
                    />
                    <Salidas
                        div="div2"
                        carrera="Hacker ético."
                        icon="fa-brands fa-redhat"
                    />
                    <Salidas
                        div="div3"
                        carrera="Chief Information Security Officer."
                        icon="fa-solid fa-user-shield"
                    />
                    <Salidas
                        div ="div4"
                        carrera="Especialista en incidencias."
                        icon="fa-solid fa-helmet-safety"
                    />
                    <Salidas
                        div = "div5"
                        carrera = "Analista de seguridad."
                        icon = "fa-solid fa-magnifying-glass-chart"
                    />
                </div>
            </div>
<div class="fondo">
    <div class="container">
            <div class="card" id="contenido-curso">
                <h1>CONTENIDO DEL CURSO</h1>
                <p>Estas son las asignaturas que cursarás a lo largo del año escolar (7 meses) que dura nuestro curso.<br>
                    El recuento computado de horas suponen un total de <b>600</b> horas. Es decir, 19 horas semanales de curso.</p>
                <div class="contenido-box">
                    <Contenido
                        div="div1"
                        titulo="Gestión de servicion en el sistema."
                        horasanuales=" 95 horas anuales"
                        horassemanales=" 3 horas semanales"
                    />
                    <Contenido
                        div="div2"
                        titulo="Acceso a sistemas y datos seguros."
                        horasanuales=" 125 horas anuales"
                        horassemanales=" 4 horas semanales"
                    />
                    <Contenido
                        div="div3"
                        titulo="Seguridad en equipos informaticos."
                        horasanuales=" 187 horas anuales"
                        horassemanales=" 5 horas semanales"
                    />
                    <Contenido
                        div="div4"
                        titulo="Gestión de incidentes de seguridad en redes."
                        horasanuales=" 125 horas anuales"
                        horassemanales=" 4 horas semanales"
                    />
                    <Contenido
                        div="div5"
                        titulo=" Auditoria de seguridad informática."
                        horasanuales=" 95 horas anuales"
                        horassemanales=" 3 horas semanales"
                    />
                </div>
            </div>
            </div>
                <hr>
            <div class="container">
                <div class="card" id="acceso-curso">
                    <h1>Acceso al Curso</h1>
                    <div class="acceso-box">
                        <Accesotable 
                            titulacion1="Técnico Superior en Administración de Sistemas Informáticos en Red "
                            titulacion2 ="Técnico Superior en Desarrollo de Aplicaciones Multiplataforma "
                            titulacion3 ="Técnico Superior en Desarrollo de Aplicaciones Web"
                            titulacion4 ="Técnico Superior en Animaciones 3D, Juegos y Entornos Interactivos "
                            subtitulacion1 ="establecido por
                            el Real Decreto 1629/2009, de 30 de octubre, por el que se establece el título de
                            Técnico Superior en Administración de Sistemas Informáticos en Red y se fijan sus
                            enseñanzas mínimas"
                            subtitulacion2="establecido por el
                            Real Decreto 450/2010, de 16 de abril, por el que se establece el título de Técnico
                            Superior en Desarrollo de Aplicaciones Multiplataforma y se fijan sus enseñanzas
                            mínimas."
                            subtitulacion3="establecido por el Real Decreto
                            686/2010, de 20 de mayo, por el que se establece el título de Técnico Superior en
                            Desarrollo de Aplicaciones Web y se fijan sus enseñanzas mínimas."
                            subtitulacion4="establecido por el
                            Real Decreto 1583/2011, de 4 de noviembre, por el que se establece el título de
                            Técnico Superior en Animaciones 3D, Juegos y Entornos Interactivos y se fijan sus
                            enseñanzas mínimas."
                        />
                    </div>
                </div>
            </div>
            <hr>
            <div class="container">
            <div class="card" id="consultar-plazas">
                <h1>Consultar Plazas</h1>
                <p class="read-more">
                    <a href="/index.php/al-dia/922-aula-ateca-disponible-ya" class="btn btn-primary">
                    Leer más...
                    </a>
                </p>
            
            </div>
    </div>
</div>
</main>

<style lang="sass">


main
    --opacidad-negro: 0.35
    background-image: linear-gradient(rgba(0, 0, 0, var(--opacidad-negro)), rgba(0, 0, 0, var(--opacidad-negro))), url(../src/images/paginas/keyboard.jpg)
    background-attachment: fixed
    background-size: cover
    background-position: center
    width:100%

.container
    padding: 0px 60px
    
.fondo
    background-color: rgb(255,255,255)

.encabezado
    color: white
    padding: 2% 0%
    h1
        font-size: 40px
        color: white
        font-weight: 500
        i
            padding-top: 2.3%
            font-size: 48px
            padding-bottom:33px
 
h1
    text-align: center
    padding: 28px
    color: #343434
    font-weight: 400

hr
    height: 12px
    border: 0
    box-shadow: inset 0 12px 12px -12px rgba(0, 0, 0, 0.5)

.card
    background-color: transparent
    border: none
    padding: 2% 0%
    margin-bottom: 4% 
    scroll-snap-align: center
    
    p
        text-align: center
        font-size:22px


.salidas-box
    width:100%
    padding: 0% 10%
    display: flex
    justify-content: space-evenly
    align-items: center
    background-color:(255,255,255,.5)


#contenido-curso
    p
        color: #595959
        font-size: 20px

.contenido-box
    width:100%
    display: flex
    justify-content: space-evenly
    

.acceso-box 
    margin: 1rem 5rem 0 0
    display: flex
    align-items: center
    width: 100%
    padding-bottom: 3%  
  
    


.btn-primary
    background-color: #22b8f0
    border-color: #22b8f0
    width:40%
    margin: 4vh


    
@media screen and (max-width: 1300px)
    .salidas-box
        width:100%
        padding: 0% 4%
        display: flex
        justify-content: space-around
        align-items: center
        background-color:(255,255,255,.5)

   
    #contenido-curso
        p
            color: #595959
            font-size: 17px

@media screen and (max-width: 1150px)
    .contenido-box
        display: flex
        justify-content: space-around
        flex-direction: row
        width: 100%
        
    
 
    .salidas-box
        width:100%
        padding: 0% 10%
        display: flex
        justify-content: space-around
        align-items: center
        flex-wrap: wrap
        background-color:(255,255,255,.5)

    .contenido-box
        display: flex
        justify-content: space-around
        flex-direction: row
        flex-wrap: wrap
        width: 100%
      
   

    


</style>