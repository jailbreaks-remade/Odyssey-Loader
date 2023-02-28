<script lang="ts">
    import spinner from '../assets/spinner.gif'
    import apple from '../assets/whiteicon.png'
    import ConsoleScreen from './ConsoleScreen.svelte';
    let showSpinner: boolean = false;
    let showApple: boolean = false;
    let showConsole: boolean = false;
    setTimeout(() => {  showSpinner = true; }, 2000);
    setTimeout(() => {  showSpinner = false, showApple = true }, 6000);
    setTimeout(() => {  showSpinner = false, showApple = false, showConsole = true }, 12000);
</script>

<div class="h-screen bg-black">
    {#if showSpinner}
        <div class="h-full w-full flex justify-center items-center">
            <img class="h-[24px]" src={spinner} alt="Loading.."/>
        </div>
    {/if}
    {#if showApple}
    <div class="h-full w-full flex justify-center items-center">
        <img class="h-[48px]" src={apple} alt="Loading.."/>
    </div>
    {/if}
    {#if showConsole}
        <ConsoleScreen/>
    {/if}

</div>