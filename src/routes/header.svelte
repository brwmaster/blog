<script lang="ts">
  import * as config from '$lib/config'
</script>

<nav>
  <a href="/" class="title">{config.title}</a>

  <ul class="links">
    <li>
      <a href="/about">about</a>
    </li>
    <li>
      <a href="/contact">contact</a>
    </li>
    <li>
      <a href="/rss.xml" target="_blank">rss</a>
    </li>
  </ul>

  <button>Toggle</button>
</nav>

<style>
  nav {
    padding-block: var(--size-7);
  }

  .links {
    margin-block: var(--size-7);
  }

  a {
    color: inherit;
    text-decoration: none;
  }

  @media (min-width: 768px) {
    nav {
      display: flex;
      justify-content: space-between;
    }

    .links {
      display: flex;
      gap: var(--size-7);
      margin-block: 0;
    }
  }
</style>
