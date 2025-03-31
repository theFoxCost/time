<script>
    import moment from "moment"; 
    import { onMount } from "svelte";
  
    let ctime = moment().format("YYYY-MM-DD HH:mm:ss");
  
    onMount(() => {
      setInterval(() => {
        ctime = moment().format("YYYY-MM-DD HH:mm:ss");
      }, 1000);
    });
  </script>
  
  <main>
    <h1>{ctime}</h1>
  </main>
  
  <style>
    h1 {
      color: black;
    }
  </style>
  