
<style></style>

<script lang="ts">
    import "../app.css";  // global styles
    import {ModeWatcher} from "mode-watcher";
    import Menu from "../Menu.svelte";
</script>

<!--For dark mode-->
<ModeWatcher/>

<Menu/>

<!--`<slot></slot>` acts as a placeholder for non-layout content.-->
<slot></slot>
