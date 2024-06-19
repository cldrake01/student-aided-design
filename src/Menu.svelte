<script lang="ts">
    import "./app.css";  // global styles
    import * as Menubar from "$lib/components/ui/menubar/index.js";

    let bookmarks = false;
    let fullUrls = true;

    const profileRadioValue = "benoit";

    import Sun from "lucide-svelte/icons/sun";
    import Moon from "lucide-svelte/icons/moon";

    import {toggleMode} from "mode-watcher";
    import {Button} from "$lib/components/ui/button/index.js";

    import * as Breadcrumb from "$lib/components/ui/breadcrumb/index.js";
    import * as DropdownMenu from "$lib/components/ui/dropdown-menu/index.js";
</script>

<Menubar.Root class="menubar">

    <!--Menubar-->
    <Menubar.Menu>
        <Menubar.Trigger><a href="/volunteer-sign-in">Volunteer Sign-in</a></Menubar.Trigger>
    </Menubar.Menu>
    <Menubar.Menu>
        <Menubar.Trigger><a href="/">About</a></Menubar.Trigger>
    </Menubar.Menu>
    <Menubar.Menu>
        <Menubar.Trigger>Requests</Menubar.Trigger>
        <Menubar.Content>
            <Menubar.Item href="/lesson-request">Lesson Request</Menubar.Item>
            <Menubar.Item href="/item-request">Item Request</Menubar.Item>
        </Menubar.Content>
    </Menubar.Menu>

    <!--    Dark Mode Toggle-->
    <!--    To add an outline, use `variant="outline"`.-->
    <Button on:click={toggleMode} variant="ghost" size="icon">
        <Sun
                class="h-[1.2rem] w-[1.2rem] rotate-0 scale-100 transition-all dark:-rotate-90 dark:scale-0"
        />
        <Moon
                class="absolute h-[1.2rem] w-[1.2rem] rotate-90 scale-0 transition-all dark:rotate-0 dark:scale-100"
        />
        <span class="sr-only">Toggle theme</span>
    </Button>

</Menubar.Root>
