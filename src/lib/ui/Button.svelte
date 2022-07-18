<script lang="ts">
  export let variant: string = "default";
  export let outline: boolean = false;
</script>

<button class={variant} class:outline>
  <slot />
</button>

<style>
  button {
    border-radius: 24px;
    border: 2px solid transparent;
    padding: 0.6em 1.2em;
    font-size: 1em;
    font-weight: 500;
    font-family: inherit;
    cursor: pointer;
    transition: border-color 0.25s, background-color 0.25s;
    color: var(--light);
  }

  button.light {
    background-color: var(--light);
    border-color: var(--light);
    color: var(--dark);
  }
  button.dark {
    background-color: var(--dark);
    border-color: var(--dark);
  }
  button.primary {
    background-color: var(--primary);
    border-color: var(--primary);
  }
  button.secondary {
    background-color: var(--secondary);
    border-color: var(--secondary);
  }
  button.success {
    background-color: var(--success);
    border-color: var(--success);
  }
  button.warning {
    background-color: var(--warning);
    border-color: var(--warning);
  }
  button.danger {
    background-color: var(--danger);
    border-color: var(--danger);
  }

  button.outline {
    background-color: transparent;
    color: inherit;
  }
  button.outline:hover {
    border-color: inherit;
  }
  button.outline.dark:hover {
    border-color: var(--light);
  }
  button.outline.light:hover {
    border-color: var(--dark);
  }

  button:hover {
    background-color: transparent;
    color: inherit;
  }

  button:focus,
  button:focus-visible {
    outline: 6px auto black;
  }
</style>
