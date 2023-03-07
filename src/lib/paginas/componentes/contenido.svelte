<script>
  export let div, titulo, horasanuales, horassemanales;
</script>

<main>
    <div class="{div}" id="contenido">
        <div class="titulo"> <h4>{titulo}</h4></div>
        <div class="arrow">▼</div>
        <div class="hideable"><h4><i class="fa-solid fa-clock"></i>{horasanuales}<br>
            <i class="fa-regular fa-clock"></i>{horassemanales}</h4>
        </div>
    </div>
</main>

<style lang="sass">
    main
        margin: 0% 1%
    #contenido
        display: grid
        grid-template-columns: 1fr
        grid-template-rows: repeat(3)
        width: 30vh
        position: relative
        margin: 1rem 2%
        color: #005D9D
        border: 8px solid #0038FF
        text-align: center
        overflow: hidden
        line-height: 150%
        transition: height .5s
        height: 10.5rem
        border-image: url("data:image/svg+xml,%3Csvg width='24' height='24' viewBox='0 0 24 24' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M16 0H8v4H4v4H0v8h4v4h4v4h8v-4h4v-4h4V8h-4V4h-4V0zm0 4v4h4v8h-4v4H8v-4H4V8h4V4h8z' fill='%23005D9D'/%3E%3C/svg%3E") 8 stretch
        h4
            padding: 23px
            font-size: 18px
        
        .titulo
            height:6.375rem
        .arrow
            height:0.2rem
        .hideable
            display: none
            height:6.35rem

    #contenido:hover
        height: 20.125rem
        color: #49ABD3
        border-image: url("data:image/svg+xml,%3Csvg width='24' height='24' viewBox='0 0 24 24' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M16 0H8v4H4v4H0v8h4v4h4v4h8v-4h4v-4h4V8h-4V4h-4V0zm0 4v4h4v8h-4v4H8v-4H4V8h4V4h8z' fill='%2349ABD3'/%3E%3C/svg%3E") 8 stretch
        
        .hideable
            display: block
            height:4.5rem
        
@media screen and (max-width: 1150px)
        #contenido
            width: 70vh
            
            
    
     
</style>