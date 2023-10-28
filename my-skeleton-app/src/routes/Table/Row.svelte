<script>
	import { ProgressRadial } from '@skeletonlabs/skeleton';
    import Status from './Status.svelte';
    import { Avatar } from '@skeletonlabs/skeleton';
    let entry = "DD/MM/YYYY HH:MM:SS";
    let ladle = "ladle";
</script>

{#each Array(100) as row, i}
    <tr>
        <td>{i+1}</td>
        <td>{ladle}</td>
        <td class="flex justify-center">
            <Status status={"Active"} />
        </td>
        <td>{entry}</td>
        <td>{entry}</td>
        <td class="flex justify-around">
            <ProgressRadial width='w-6' stroke='200' value = 10/> 
            <span>1000</span>
                <!-- <ProgressBar label="Progress Bar" value={50} max={100} /> -->
        </td>
    </tr>
{/each}