<script>
  import { Link } from "svelte-navigator";
</script>

<nav>
  <div class="navbar">
    <Link to="/">Pakkeliste</Link>
    <Link to="/components">Komponenter</Link>
  </div>
</nav>

<style>
  nav {
    width: 100%;
    padding-block: 12px;
    padding-inline: 8px;
    background-color: var(--primary);
  }

  @media (min-width: 320px) {
    nav {
      padding-inline: 5.625%;
    }
  }

  .navbar {
    display: flex;
    flex-direction: row;
    gap: 40px;
    color: var(--light);
    min-width: 320px;
    max-width: 1584px;
    margin-inline: auto;
  }

  :global(.navbar a) {
    color: white;
    text-decoration: none;
  }
</style>
