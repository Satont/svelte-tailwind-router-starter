<script lang="ts">

  import { Router, Route } from "svelte-navigator";
  import Main from './pages/Main.svelte'
  import Dashboard from './pages/Dashboard.svelte'
</script>

<h1 class="text-3xl font-bold underline">
  Hello world!
</h1>

<Router>
  <Route path="dashboard/*">
    <Route path="/" component={Dashboard} />
  </Route>

  <Route component={Main} />
</Router>

<style>

</style>
