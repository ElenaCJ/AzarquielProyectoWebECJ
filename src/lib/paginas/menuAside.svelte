<script>
    document.querySelectorAll('#temario .lista a').forEach((elemento) => {
        elemento.addEventListener('click', () => {
            document.querySelector('#temario .activo').classList.remove('activo');
            elemento.parentElement.classList.add('activo');
        });
    });
</script>

<main>
    <aside>
        <div class="contenedor-temario" id="temario">
            <ul class="lista">
                <li><a href="#competencias-generales">competencias generales</a></li>
                <li><a href="#salidas-profesionales">salidas profesionales</a></li>
                <li><a href="#contenido-curso">contenido del curso</a></li>
                <li><a href="#acceso-curso">acceso al curso</a></li>
                <li><a href="#consultar-plazas">consultar plazas</a></li>
            </ul>
        </div>
    </aside>
</main>

<style lang="sass">
     
   
main
    position: sticky
    z-index: 5
    width:100%
    top: calc(42% - (195px / 2))
aside
    position: sticky
    padding: 0% 2% 1.5% 0%
    z-index: 5
    width: 14%
    left: 100%
    transform: translateX(2rem)
    transition: .5s
    .lista
        text-align: right
        opacity: 1
        transform: perspective(600px) rotateY(-65deg)
        transition: .5s 
        
    .lista:hover
        transform: perspective(600px) rotateY(0deg)
        opacity: 1
        background-color: white 

aside:hover
    transform: translateX(0rem)
    


ul 
    padding: 0% 7% 15% 0%
    position: absolute
    flex-direction: column
    align-items: start
    list-style-type: none

    a 
      position: relative
      display: block
      padding: 15px 0
      font-family: sans-serif
      color: #009BDD
      opacity:0.6
      text-decoration: none
      text-transform: uppercase
      transition: 0.5s
      

      &::after 
        position: absolute
        content: ""
        top: 85%
        right: 0
        width: 100%
        height: 3px
        background: #3498db
        transform: scaleX(0)
        transform-origin: right
        transition: transform 0.5s
        opacity: 1
      

      &:hover 
        color: #009CDC
        opacity: 1
      

      &:hover::after 
        transform: scaleX(1)
        transform-origin: left
        opacity: 1



</style>