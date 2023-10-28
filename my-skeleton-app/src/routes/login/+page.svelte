<script>
    let user="";
    let pass="";
    const makelogin = (event) =>{
        window.location.href = '/Table';
    }
</script>

<!-- {#if destroy} -->
    <div class="login" on:submit={makelogin}>
        <h2 class="text-5xl login-text">-LOGIN-</h2>
        <form class="form">
            <input 
                class="input variant-form-material pad margin" 
                title="Input (text)" 
                type="text" 
                placeholder="Username" 
                bind:value={user}/>
            <input 
                class="select variant-form-material pad margin" 
                title="Input (text)" 
                type="password" 
                placeholder="Password" 
                bind:value={pass}/>
            <button class="btn variant-filled-primary center pad rounded-md" type="submit" href="/Table">
                Submit
            </button>
        </form>
    </div>
<!-- {/if} -->

<style>
    .btn{
        position: relative;
        left:27%;
        width:100px;
    }

    .login{
        position: fixed;
        top: 30%;
        left: 40%;
    }

    .pad{
        margin: 10px;
    }

    .form{
        display: flex;
        justify-content: center;
        flex-direction: column;
    }

    .login-text{
        position: relative;
        left: 17%;
        margin-bottom: 10px;
    }
</style>
