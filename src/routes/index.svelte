<script>
  import CovidStat from '../components/CovidStat.svelte';
  import CovidChart from '../components/CovidChart.svelte';
  import TableContainer from '../components/TableContainer.svelte';
</script>
<svelte:head>
  <title>Home | Covid Tracker</title>
</svelte:head>
<CovidStat />

<CovidChart />

<TableContainer />

<div class="container">
  <div class="columns is-centered is-mobile is-vcentered">
    <div class="column is-10">
      <h1 class="title has-text-centered">Covid Tracker</h1>
    </div>
  </div>
</div>
<style>
</style>
