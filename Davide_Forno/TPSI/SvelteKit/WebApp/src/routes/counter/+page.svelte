<script>
    import Counter from "../../lib/components/counter.svelte";
    let contatore = 0;
    import DCounter from "../../lib/components/Double_counter.svelte";
    let Dcontatore = 0;
</script>
<h1>Pagina Counter!!!</h1>
<h2>Il valore del contatore vale: {contatore}</h2>
<Counter bind:counter={contatore}/>

<h2>Il valore del contatore Double vale: {Dcontatore}</h2>
<DCounter bind:counter={Dcontatore}/>