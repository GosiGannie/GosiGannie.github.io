<h1>Registration Form</h1>

<form on:submit|preventDefault={handleSubmit}>
    <label for='firstName'>First Name:</label>
    <input id='firstName' type='text'/>
    <label for='lastName'>Last Name:</label>
    <input id='lastName' type='text'/>
    <label for='email'>Email:</label>
    <input id='email' type='email'/>
    <label for='password'>Password:</label>
    <input id='password' type='password'/>

    <button type='submit'>Register</button>
 </form>

 <script>
    function handleSubmit() {
        let name = 'Form Submitted!';
        console.log(name);
    }
</script>

<style>
    form{display: grid;
    width: 60%;
    max-width: 500;
    min-width: 300;
    margin: auto;
    grid-template-columns: repeat(2, minmax(200px, 1fr));
    }
    :global(body){
        background-color: #EEC5DF;
    }
</style>
