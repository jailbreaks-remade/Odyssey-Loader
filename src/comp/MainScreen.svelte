<script lang="ts">
    import '../app.css'
    import JailbreakingScreen from './JailbreakingScreen.svelte';
    import Tablerow from './Tablerow.svelte';
  
    let jailbreaking: boolean = false;
    let showJBScreen: boolean = false;
      const runJB = () => {
        jailbreaking = true;
        setTimeout(() => {  jailbreaking = false; }, 3000);
        setTimeout(() => {  showJBScreen = true; }, 3000);
      }
      
  </script>
  
{#if !showJBScreen}
<main class="flex justify-center h-screen items-center flex-col w-full">
    <h1 class="odyssey w-full grid place-items-center">Odyssey</h1>
    <div class="p-[2.5rem]">
      <div on:click={runJB} class="rounded-full w-[180px] h-[180px] border-[4px] font-semibold active:touch-none active:scale-[99%] flex justify-center items-center">{#if jailbreaking}Jailbreaking...{:else}Jailbreak{/if}</div>
    </div>
    <div class="table rounded-2xl h-[26%] w-[60%] shadow-xl">
      <Tablerow toggleButton text="Enable Tweaks"/>
      <Tablerow toggleButton text="Restore RootFS"/>
      <Tablerow text="Settings"/>
      <Tablerow text="Credits"/>
    </div>
  </main>
  {:else}
  <JailbreakingScreen/>
{/if}
  