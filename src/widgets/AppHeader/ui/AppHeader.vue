<script lang="ts" setup>
import glasses from "@/shared/icons/glasses.vue";
import exit from "@/shared/icons/exit.vue";

import AppBtn from "@/shared/ui/AppBtn.vue";
</script>

<template>
  <div class="header">
    <div class="container">
      <div class="header__content">
        <router-link to="/" class="header__logo">
          <img src="@/shared/img/logo/2-light.png" alt="Лимон" />
        </router-link>
        <div class="header__btns">
          <a-divider type="vertical" class="divider" />
          <AppBtn class="text">
            <glasses />
          </AppBtn>

          <a-divider type="vertical" class="divider" />
          <AppBtn class="text white">
            Вход
            <exit />
          </AppBtn>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.header {
  background-color: var(--dark-color-2);

  &__content {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-top: 12px;
    padding-bottom: 12px;
  }

  &__logo {
    width: 150px;
  }

  &__btns {
    display: flex;
    gap: 20px;
  }
}
.divider {
  height: auto;
  background-color: #fff;
  margin: 8px 0;
}
</style>
