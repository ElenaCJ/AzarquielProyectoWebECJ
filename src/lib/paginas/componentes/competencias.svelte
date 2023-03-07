<script>
export let src, competenciastext;
</script>

<main>
    <div class="fondo">
        <div class="container">
            <div class="card" id="competencias-generales">
                    <h1>COMPETENCIAS GENERALES</h1>
                    <div class="competencias-box">
                    <div class="img"> <img src="{src}" alt=""></div>
                    <div class="p"> <p>{competenciastext}</p>
                        </div>
                    </div>
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

    h1
        text-align: center
        padding: 28px
        color: #343434
        font-weight: 400
    .container
        padding: 0px 60px

    .card
        background-color: transparent
        border: none
        padding: 2% 0%
        margin-bottom: 4% 
        scroll-snap-align: center
        p
            text-align: center
            font-size:22px

    .fondo
        background-color: rgb(255,255,255)
    .competencias-box
        display: flex
        flex-direction: row
        justify-content: center
        align-items: center
        width: 100%
        padding-bottom: 3%
    
    .img
        width: 50%
        border: 8px solid #0038FF
        border-image: url("data:image/svg+xml,%3Csvg width='24' height='24' viewBox='0 0 24 24' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M16 0H8v4H4v4H0v8h4v4h4v4h8v-4h4v-4h4V8h-4V4h-4V0zm0 4v4h4v8h-4v4H8v-4H4V8h4V4h8z' fill='%23005D9D'/%3E%3C/svg%3E") 8 stretch
        transition: .2s
        img
            width:100%
            height: auto
    .img:hover
        border-image: url("data:image/svg+xml,%3Csvg width='24' height='24' viewBox='0 0 24 24' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M16 0H8v4H4v4H0v8h4v4h4v4h8v-4h4v-4h4V8h-4V4h-4V0zm0 4v4h4v8h-4v4H8v-4H4V8h4V4h8z' fill='%23009BDD'/%3E%3C/svg%3E") 8 stretch
    .p 
        width: 80%
        p
            font-size: 23px
            padding: 2.7% 1% 0 7%
            color: #005B9B
            text-align: center
    

       
@media screen and (max-width: 1150px)
    .card
        background-color: transparent
        border: none
        padding: 2% 0%
        margin-bottom: 4% 
        scroll-snap-align: center
        
        p
            text-align: center
            font-size:18px
            margin-bottom: 3rem
    .competencias-box
        display: flex
        justify-content: space-around
        flex-direction: column
        flex-wrap: wrap
        .img
            width: 65%
            border: 8px solid #0038FF
            border-image: url("data:image/svg+xml,%3Csvg width='24' height='24' viewBox='0 0 24 24' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M16 0H8v4H4v4H0v8h4v4h4v4h8v-4h4v-4h4V8h-4V4h-4V0zm0 4v4h4v8h-4v4H8v-4H4V8h4V4h8z' fill='%23005D9D'/%3E%3C/svg%3E") 8 stretch
            transition: .2s
            img
                width:100%
                height: auto

        .p
            width: 100%
            p
                font-size: 20px
@media screen and (max-width: 400px)
    .competencias-box
        .p
            p
                font-size: 14px
      

</style>