<script>
  // @ts-nocheck

  import FeedbackItem from "./FeedbackItem.svelte";

  export let feedback;

  console.log(feedback);
</script>

{#each feedback as feed (feed.id)}
  <FeedbackItem item={feed} on:delete-feedback />//catch the custon event
{/each}

FeedbackList
