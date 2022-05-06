<script>
  import EventComponent from "./EventComponent.svelte";

  function handleMessage(event) {
    alert(event.detail.text);
  }
</script>

<main>
  <p>Event communication.</p>
  <hr />

  <EventComponent on:message={handleMessage} />
</main>
