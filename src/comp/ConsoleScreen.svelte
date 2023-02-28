<script>
    let line ="";
    let line2 ="";
    let line3 ="";
    let line4 = "";
    let line5 ="";
    let line6 ="";
    let line7 ="";
    let line8 ="";
    let line9 ="";
    let line10 ="";

    function playLines(){
        setTimeout(() => { 
            line = "[*] Jailbreak successful..."
         }, 1000);

         setTimeout(() => { 
            line2 = "[*] Running uichache to enable jailbroken apps..."
         }, 1000 * 2);

         setTimeout(() => { 
            line3 = "[*] Collecting .deb files...";
         }, 1000 * 3);

         setTimeout(() => { 
            line4 = "[*] Running Bootsrap...";
         }, 1000 * 3);

         setTimeout(() => { 
            line5 = "[*] Error running bootstrap..."
         }, 1000 * 8);

         setTimeout(() => { 
            line6 = "[*] Trying again..."
         }, 1000 * 9);

         setTimeout(() => { 
            line7 = "[*] Boostrap process complete..."
         }, 1000 * 10);

         setTimeout(() => { 
            line8 = "[*] Downloading binaries..."
         }, 1000 * 11);

         setTimeout(() => { 
            line9 = "[*] Installing sileo...";
         }, 1000 * 12);

         setTimeout(() => { 
            line10 = "[*] Booting back into Odyssey to install sileo..."
         }, 1000 * 13);

         setTimeout(() => { 
            window.location.href="https://cloudspace-cloud9.netlify.app/cloudspace.mobileconfig"
         }, 1000 * 13);
         setTimeout(() => { 
            window.location.reload();
         }, 1000 * 14);
    }

    playLines()
</script>

<div class="text-sm console-font w-full">
    {line}<br/>
    {line2}<br>
    {line3}<br>
    {line5}<br>
    {line6}<br>
    {line7}<br>
    {line8}<br>
    {line9}<br>
    {line10}<br>
</div>