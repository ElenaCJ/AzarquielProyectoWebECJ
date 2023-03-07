<script>
    export let div, carrera, icon;
</script>

<main>
    <div class="{div}" id="salida"> 
        <div class="carrera"> <h5>{carrera}</h5></div>
        <div class="icon"><i class="{icon}"></i></div>
    </div>
</main>

<style lang="sass">
    #salida
        max-width: 200px
        margin: auto
        display: grid
        grid-template-columns: 1fr
        grid-template-rows: repeat(2, 0.8fr)
        color: white
        text-align: center
        padding-top: 2%
        .carrera
            height: 75px
            text-align: center

        .icon
            padding: 4% 4%
            font-size: 48px
    .div1
        animation: Slide_Up 4s ease
    .div2
        animation: Slide_Up 4s ease
    .div3
        animation: Slide_Up 4s ease
    .div4
        animation: Slide_Up 4s ease
    .div5
        animation: Slide_Up 4s ease

        
@keyframes Slide_Up
    0% 
        transform: translateY(150px)
    
    100% 
        transform: translateY(0px)

</style>