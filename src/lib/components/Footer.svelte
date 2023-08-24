<!-- src/lib/components/Footer.svelte  -->
<script>
  let copy = "keziah hobbs";
  let year = "2023";
</script>

<footer>&copy; {copy} &nbsp;{year}</footer>

<style lang="scss">
  footer {
    display: flex;
    justify-content: center;
    align-items: center;
    color: var(--primary);
    font-weight: bold;
    padding: 0.25em;
  }
</style>
