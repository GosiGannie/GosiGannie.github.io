<title>Spotifi Login</title>

<h1>Spotifi</h1>

<svelte:head>
  <link rel="stylesheet" href="/pico.min.css" />

  <style>
    nav {
      visibility: hidden;
    }
  </style>
</svelte:head>

<div class="login">
    <div class="login-box">
        <p style="font-size: 40px; margin-top: 50px;"><strong>Login to Spotifi</strong></p>
        <form on:submit|preventDefault={handleSubmit} id="center">
            <input id="username" type='text'class='input-box'placeholder='Username' style="background-color: rgb(185, 131, 255); margin-top: 30px"/>
            <input id="password" type="password" class='input-box'placeholder="Password" style="margin-top: 30px; background-color: rgb(185, 131, 255);"/>
            <button type="submit" style=
            "font-size: 20px;
            margin-top: 35px;
            width: 139px;
            background-color: rgb(185, 131, 255);">
            Login</button>
        </form>
    </div>
</div>

<script>
    function handleSubmit() {
        let name = 'Form Submitted!';
        console.log(name);
        window.location.href = '/spotifi-homepage'
    }
</script>

<style>
    body {
        background-image: linear-gradient(rgb(185, 131, 255), white);
        height: 935px;
    }
    .login-box {
        border: 5px solid;
        margin: auto;
        width: 700px;
        height: 510px;
        background-color: white;
        text-align: center;
        border-radius: 2%;
        box-shadow: 0 4px 80px 0 rgba(0, 0, 0, 0.2), 0 4px 80px 0 rgba(0, 0, 0, 0.2);
    }
    .input-box {
        width: 260px;
        height: 38px;
    }
    #center {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    h1 {
        text-align: center;
        font-size: 70px;        
    }
    ::placeholder {
        color: white;
    }
</style>