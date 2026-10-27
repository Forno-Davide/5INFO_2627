<svelte:head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0&icon_names=keyboard_arrow_down" />
</svelte:head>
<script>
export let nome = "";
</script>
<style>
.Drop{
    position: relative;
    width: 170px;
    padding: 10px;
    padding-left: 20px;
    color: white;
    background-color: red;
    border-radius: 15px;
    text-align: center;
    font-size: 30px;
    font-weight: bold;
    margin: 40px 0 40px 0;
}
.material-symbol-outlined{
    background-color: white;
}
</style>

<div class="Drop">{nome} <span class="material-symbols-outlined">
    keyboard_arrow_down
    </span></div>