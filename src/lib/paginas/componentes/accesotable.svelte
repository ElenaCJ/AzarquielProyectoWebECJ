<script>
    export let titulacion1, titulacion2, titulacion3, titulacion4, subtitulacion1, subtitulacion2, subtitulacion3, subtitulacion4;
</script>

<main>
    <div id="table">
        <table class="table" style="margin: 2vh;">
            <tbody>
            <tr>
                <th scope="row"> <span style="color:#343434">{titulacion1} </span>{subtitulacion1}</th>
            </tr>
            <tr>
                <th scope="row"> <span style="color:#343434">{titulacion2} </span>{subtitulacion2}</th>
            </tr>
            <tr>
                <th scope="row"> <span style="color:#343434">{titulacion3} </span>{subtitulacion3}</th>
            </tr>
            <tr>
                <th scope="row"> <span style="color:#343434">{titulacion4} </span>{subtitulacion4}</th>
            </tr>
            
            </tbody>
        </table>
        </div>
</main>

<style lang="sass">
th
    font-size:18px
    color: #005B9B
    transition: .2s

th:hover
    color: #49ABD3
table
    width: 100%

</style>