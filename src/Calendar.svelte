<script lang="ts">
    import { setContext } from 'svelte'

    setContext("type", "lesson")

    import {getLocalTimeZone, today} from "@internationalized/date";
    import {RangeCalendar} from "$lib/components/ui/range-calendar/index.js";

    const start = today(getLocalTimeZone());
    const end = start.add({days: 7});

    let value = {
        start,
        end
    };
</script>

<div class="horizontal-center">
    <RangeCalendar bind:value class="rounded-md border"/>
</div>
