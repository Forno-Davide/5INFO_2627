<script>
    import Counter from "../../lib/components/counter.svelte";
    let contatore = 0;
    import DCounter from "../../lib/components/Double_counter.svelte";
    let Dcontatore = 0;
    let numeri = [1,3,2,4,5,6,9]
    let sottolineato = true
    let Dsottolineato = true
    let doppio;
    $: doppio = contatore * 2
    $: Dcontatore % 2 ? Dsottolineato = false : Dsottolineato = true
    $: contatore == 7 ? sottolineato = false : sottolineato = true
    function gestisci_evento(evento){
        alert(`${evento.detail.tipo} -- ${evento.detail.valore}`);
    }
</script>
<h1>Pagina Counter!!!</h1>
<h2 class:sottolineato >il valore del contatore vale: {contatore}</h2>
<Counter bind:counter={contatore} on:contatore = {gestisci_evento}/>
<h2 class = "blue" >il doppio del contatore vale {doppio}</h2>
<h2 class:Dsottolineato>Il valore del contatore double vale: {Dcontatore}</h2>
<DCounter bind:counter={Dcontatore} on:Dcontatore = {gestisci_evento}/>
<ul>
    {#each numeri as numero, indice}
    <li>numeri[{indice}]:{numero}</li>
    {/each}
</ul>
<style>
.blue{color: blue;}
.rosso { color: red;}
.verde { color: green;}
.arancione{color: orange}
.sottolineato{text-decoration: underline;}
.Dsottolineato{text-decoration: underline;}
</style>
