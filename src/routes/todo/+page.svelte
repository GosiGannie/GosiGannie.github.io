<div class='container'>
    <h1>TODO LIST</h1>
        <form on:submit|preventDefault={handleSubmit}>
            <label for='input'>TODO:</label>
            <input id='input' type='text'/>
        </form>
    <div class='layout'>
        <div style='display:grid'>
            <h1>NEW</h1>
        </div>
        <div style='display:grid'>
            <h1>COMPLETED</h1>
        </div>
    </div>
</div>

<script>
    function handleSubmit() {
        let name = 'Form Submitted!';
        console.log(name);
    }
</script>

<style>
    .container{
        width: 80vw;
        height: 70vh;
        background-color: cornflowerblue;
        border-width: 10px;
        border-style: solid;
        border-color: black;
        border-radius: 3%;
        padding-top: 10px;
    }
</style>