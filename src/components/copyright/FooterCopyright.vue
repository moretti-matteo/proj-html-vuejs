<template>
  <div class="copy">
    <span><i class="fa-regular fa-copyright"></i>Copyright 2012 - 2020 | Avada Theme by <a href="">Theme Fusion</a> |
      All Rights
      Reserved | Powered by <a href="">WordPress</a></span>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.copy {
  color: var(--color-lightdark);
  width: 100%;

  svg {
    margin-right: 5px;
  }

  a {
    color: black;
    text-decoration: none;

    &:hover {
      color: var(--primary-color);
    }
  }
}
</style>