<script lang="ts">
  import "./navBar.css";
  import { onMount } from "svelte";

  /*manages the dropdown menu */
  let isDropdownOpen = false;

  const handleDropdownClick = (event: MouseEvent) => {
    event.stopPropagation();
    isDropdownOpen = !isDropdownOpen;
  };

  const closeDropdown = (event: MouseEvent) => {
    const target = event.target as HTMLElement;

    if (!target.closest(".nav-container")) {
      isDropdownOpen = false;
    }
  };

  onMount(() => {
    document.addEventListener("click", closeDropdown);

    return () => {
      document.removeEventListener("click", closeDropdown);
    };
  });
</script>

<header class="headerForNav">
  <div class="header-content">
    <a href="#top" aria-label="Home">
      <div class="logo" style:background-image="url('./webp/logo_v2.webp')">
      </div>
    </a>

    <!-- Desktop view dropdown -->
    <nav class="navbar">
      <a class="navText" href="#about">About</a>
      <a class="navText" href="#reference">Reference</a>
      <a class="navText" href="#team">Team</a>
    </nav>

    <!-- Mobile view dropdown -->
    <div class="mobile-nav-button">
      <button class="buttonNavDropdown {isDropdownOpen ? 'change' : ''}" on:click={handleDropdownClick} aria-label="Toggle navigation menu">
        <div class="bar1"></div>
        <div class="bar2"></div>
        <div class="bar3"></div>
      </button>

    </div>
  </div>
  {#if isDropdownOpen}
    <nav class="dropdown-content">
      <a href="#about" class="navText" on:click={handleDropdownClick}>About</a>
      <a href="#reference" class="navText" on:click={handleDropdownClick}>Reference</a>
      <a href="#team" class="navText" on:click={handleDropdownClick}>Team</a>
    </nav>
  {/if}
</header>
