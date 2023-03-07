<script>
    export let text, titulo, href, id;
</script>

<main>
        <a {href}>
            <div class="box" id={id} >
                <h3>{titulo}</h3>
                <i class="fa fa-graduation-cap"></i>
                <section>{text}</section>
            </div>
        </a>
</main>

<style lang="sass">
    a
        text-decoration: none
        color: #fff
        
    main
        background-color: #fff
        text-align: center
        -webkit-font-smoothing: antialiased
        font-family: Open Sans, sans-serif
        line-height: 1.5rem
        margin-bottom: 4%


    .box
        height: 22rem
        padding:3.5rem
        margin:3%
        width:90%
        box-shadow:0 2px 3px 0px rgba(0,0,0,0.25)
        border-radius:5px
        transition:.2s all
        background: #009CDE
       
    #ciber
        background-image: url(../images/fondo-ciber_noact.jpg)
        background-repeat: no-repeat
    #videoj
        background-image: url(../images/fondo-videojuegos_no.jpg)
        background-repeat: no-repeat

    .box:hover
        height: 24rem
        padding: 3.5em
   
   
    #ciber:hover
        background-image: url(../images/fondo-ciber.jpg)
        backgroung-size: cover
        background-position: center
        background-repeat: no-repeat
        

    #videoj:hover
        background-image: url(../images/fondo-videjuegos.jpg)
        backgroung-size: cover
        background-position: center
        background-repeat: no-repeat
    
    h3
        font-weight: 650
        text-decoration: underline
        letter-spacing:2px
    
.fa-graduation-cap
    font-size: 2.4rem
    margin: 1.2rem
    
    
@media screen and (max-width: 1300px)
    #ciber
        backgroung-size: 12vh 40vh
        background-image: url(../images/fondo-ciber_noact.jpg)
        background-repeat: no-repeat
    #videoj
        backgroung-size: 12vh 40vh
        background-image: url(../images/fondo-videojuegos_no.jpg)
        background-repeat: no-repeat
    
    #ciber:hover
        background-image: url(../images/fondo-ciber.jpg)
        backgroung-size: 12vh 40vh
        background-position: center
        background-repeat: no-repeat
        

    #videoj:hover
        background-image: url(../images/fondo-videjuegos.jpg)
        backgroung-size: cover
        background-position: center
        background-repeat: no-repeat
</style>