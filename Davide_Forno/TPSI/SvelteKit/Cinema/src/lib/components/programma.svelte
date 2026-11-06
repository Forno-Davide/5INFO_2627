<script>
export let nome_cinema;
export let durata;
export let genere;
export let ora;
export let prezzo;
export let sala;
</script>
<style>
.programma{
    position: relative;
    border: solid black 3px;
    width: 300px;
    font-size: 20px;
    padding: 20px;
}
</style>
<div class="programma">
<b>{nome_cinema}</b><br><br>
{genere} - {durata} min<br><br>
sala {sala} - {ora}<br><br>
{prezzo}<br><br>
<a href="/sala">scegli posti</a>
</div>