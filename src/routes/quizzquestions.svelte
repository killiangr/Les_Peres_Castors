<script>
import Header from "$lib/Header.svelte";

</script>
<head>
    <link href="../lib/styles.css" rel="stylesheet">
    <script defer src="../lib/script.js"></script>
    <title>Quizz</title>
  </head>
  
  <Header/>
  <body class="min-w-screen">
    <div class="relative min-h-screen min-w-screen">
      <div class="z-10 relative bg-white min-h-screen mt-5 w-full">
        <iframe
          class="relative min-h-screen"
          title="Quizz"
          width="100%"
          height="100%"
          src="https://team-rcv.xyz/lpc/quizz"
        />
      </div>
    </div>
  </body>