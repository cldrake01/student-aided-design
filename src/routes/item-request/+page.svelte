<script lang="ts">
    import {setContext} from "svelte";
    import {Textarea} from "$lib/components/ui/textarea";

    setContext("type", "item")

    let step = 0;

</script>

{#if step === 0}
    <div class="horizontal-center vertical-center">
        <h3 class="item">Describe what it is that you'd like designed and built.</h3>
        <Textarea class="text-field" placeholder="Type your message here."/>
    </div>
{/if}
