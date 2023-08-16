<script setup lang="ts">
  import LogoEdMachina from './icons/LogoEdMachina.vue'
  import Language from './icons/IconLanguage.vue'
  import DarkMode from './icons/IconDarkMode.vue'
  import Notifications from './icons/IconNotifications.vue'
</script>

<template>
  <header>
    <LogoEdMachina class="header__logo"></LogoEdMachina>
    <section>
      <div class="header__options">
        <Language></Language>
        <DarkMode></DarkMode>
        <Notifications></Notifications>
      </div>
      <div class="header__info">
        <div>
          <span>Hellen Smith</span>
          <span>Admin</span>
        </div>
        <figure>
          <img src="../assets/adminavatar.png">
          <div></div>
        </figure>
      </div>
    </section>
  </header>
</template>

<style scoped>
  header {
    display: flex;
    background-color: var(--primary);
    align-items: center;
    justify-content: space-between;
    padding: 0.75rem;
    font-size: 0.5rem;
    color: var(--bg-light);
  }

  .header__logo {
    transform: scale(0.7);
  }
  section, .header__info, .header__options {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 0.5rem;
  }

  .header__info div {
    display: flex;
    flex-direction: column;
    font-weight: 700;
    text-align: end;
  }
  .header__info figure {
    margin: 0;
  }

  .header__info img {
    border-radius: 50%;
    border: 1.5px solid var(--secondary);
    position: relative;
    top: 0.5rem;
  }

  .header__info figure div {
    border-radius: 50%;
    width: 8px;
    height: 8px;
    background-color: var(--green);
    position: relative;
    bottom: 0.5rem;
    left: 2rem;

  }

  @media (min-width: 768px) {
    header {
      padding: 0.75rem 1.375rem;
      font-size: 0.75rem;
    }

    .header__logo {
      transform: none;
    }

    section, .header__info, .header__options {
      gap: 1rem;
    }
  }


</style>

