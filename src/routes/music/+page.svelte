<title>MusicPlayer</title>

<h1>Spotifi</h1>

<div class="logIn">
    <div class="center">
        <form on:submit|preventDefault={handleSubmit}>
            <input id="userName" type='text'placeholder='Username' style="margin-top:20px;"/>
            <input id="password" type="text" placeholder="Password" style="margin-top: 20px;"/>
            <button type="submit" style=
            "font-size: 20px;
            font-family:'Times New Roman', Times, serif;
            margin-top: 20px">
            Login</button>
        </form>
    </div>
</div>

<script>
    function handleSubmit() {
        let name = 'Form Submitted!';
        console.log(name);
    }
</script>

<style>
    form {
        text-align: center;
        font-size: 20px;
        background-color: rgb(205, 152, 255);
        width: 200px;
        height: auto;
        padding-bottom: 10px;
    }
    .center {
        border: 5px solid;
        margin: auto;
        width: 200px;
    }
    h1 {
        text-align: center;
        font-size: 70px;        
    }
</style>