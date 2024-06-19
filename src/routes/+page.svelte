<script lang="ts">
    import * as Accordion from "$lib/components/ui/accordion/index.js";
    import {Layout} from "lucide-svelte";
</script>

<div class="horizontal-center">
    <Accordion.Root class="w-full sm:max-w-[70%] item">
        <Accordion.Item value="item-1">
            <Accordion.Trigger>What items can we create?</Accordion.Trigger>
            <Accordion.Content>
                Anything our engineers can design, and anything that doesn't require obscure filaments.
            </Accordion.Content>
        </Accordion.Item>
        <Accordion.Item value="item-2">
            <Accordion.Trigger>What age groups do we offer lessons for?</Accordion.Trigger>
            <Accordion.Content>
                We offer lessons for grades 4-10.
            </Accordion.Content>
        </Accordion.Item>
        <Accordion.Item value="item-3">
            <Accordion.Trigger>What's our timeline?</Accordion.Trigger>
            <Accordion.Content>
                If you can attach `.stl` files, under a week. Otherwise, one to two weeks for items and lesson plans.
            </Accordion.Content>
        </Accordion.Item>
    </Accordion.Root>
</div>
