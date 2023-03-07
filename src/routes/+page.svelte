<script>
  import CardInicio from "../lib/cardInicio.svelte";


</script>

<main>
    <section class="titulo">
        <h1>
            Nuestras Novedades en Cursos de Especialización:
        </h1>
    </section>
    <div class="box-wrap">
       <CardInicio
            href = "/ciberseguridad"
            id = "ciber"
            titulo ="CIBERSEGURIDAD"
            text ="Este programa pretende formar en temas como la ciberinteligencia, el malware o  el hacking ético.
            Comprendiendo a su vez los fundamentos de la ciberseguridad y el cibercrimen, permitirá a su vez analizar software y así, construir una arquitectura 
            implementada ante incidentes y potenciales peligros."
        />
        <CardInicio
            href = "/videojuegos"
            id = "videoj"
            titulo ="VIDEOJUEGOS"
            text ="En esta formación aprenderás a diseñar y desarrollar videojuegos para diferentes dispositivos y plataformas, asegurando la experiencia del
            usuario mediante herramientas de última generación que actuaran en todas las
            fases del desarrollo, así como aplicaciones interactivas de realidad virtual y aumentada."
        
        /> 
    </div>
</main>


<style lang="sass">
   
    .titulo
        h1
            color:#009CDC
            font-weight: 800
            text-decoration: underline
            margin: 2.5rem
            margin-top: 3rem
            margin-bottom: 1.2rem
    main
        background-color: #fff
        text-align: center
        -webkit-font-smoothing: antialiased
        font-family: Open Sans, sans-serif
        line-height: 1.5rem
        margin-bottom: 4%

    .box-wrap
        color: #fff
        display: flex
        align-items: center
        justify-content: center
        margin: 0 8%

   

    .box-wrap:hover
        opacity:.6
        transform: scale(.98)
        box-shadow: none
        

    .box-wrap:hover 
        transform: scale(1)
        opacity:1
        transition: all 0.5s ease-out

    
    
@media screen and (max-width: 1300px)
    .box-wrap
        color: #fff
        display: flex
        align-items: center
        justify-content: center
        flex-wrap: wrap
        margin: 0 8%



</style>