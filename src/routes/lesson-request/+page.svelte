<script lang="ts">
    import {Textarea} from "$lib/components/ui/textarea";

    let step = 0;

</script>

{#if step === 0}
    <div class="horizontal-center vertical-center">
        <h3 class="item">
            Describe to us what sort of lesson plan you'd like and how we can integrate it into your curricula.
        </h3>
        <Textarea class="text-field" placeholder="Type your message here."/>
        <h3 class="item">
            Please include links to material that we'd be integrating with.
        </h3>
        <Textarea class="text-field" placeholder="Type your message here."/>
    </div>
{/if}
