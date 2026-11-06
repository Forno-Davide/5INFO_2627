<script>
export let n_domanda = 1;
export let risposte = ["si","no","forse","non lo so"];
export let domande_tot = 6;
export let domanda = "di che colore era il cavallo bianco di napoleone";
export let esito_risposta = false;
</script>
<style>
nav ul{
    list-style: none;
}
</style>
<p>Domanda {n_domanda} di {domande_tot}</p>
<p>{domanda}</p>
<ul>
<li><button>{risposte[0]}</button></li>
<li><button>{risposte[1]}</button></li>
<li><button>{risposte[2]}</button></li>
<li><button>{risposte[3]}</button></li>
</ul>
