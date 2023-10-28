<script>
    import Navbar from "../Navbar.svelte";
    let destroy = true;
    let user="";
    let pass="";
    const close = () =>{
        // console.log(user+" "+pass);
        destroy = false;
    }
</script>

{#if destroy}
    <form class = "modal">
        <input class="input variant-form-material" title="Input (text)" type="text" placeholder="Username" bind:value={user}/>
        <input class="select variant-form-material" title="Input (text)" type="password" placeholder="Password" bind:value={pass}/>
        <button class="btn variant-filled-primary" on:click={close} href="/Table.svelte">Submit</button>
    </form>
{/if}
