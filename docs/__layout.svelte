<script lang="ts">
  import Menu from "$lib/docs/menu.svelte";
  import MobileMenu from "$lib//docs/mobile-menu/index.svelte";
  import Search from "$lib/docs/search.svelte";
  import "../../src/assets/markdown-commons.scss";
  import { MENU } from "./menu";
</script>

<div class="pb-10 md:flex md:pt-10">
  <div class="hidden md:block md:w-1/3 md:pt-24 md:pr-8">
    <Menu {MENU} />
  </div>
  <div class="md:w-2/3">
    <Search />
    <MobileMenu {MENU} />
    <slot />
  </div>
</div>
