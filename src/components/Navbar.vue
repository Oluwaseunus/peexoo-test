<template>
  <div class="nav">
    <div></div>
    <div class="nav--link">
      Explore photos
    </div>
    <div class="nav--link">
      Find a photographer
    </div>
    <div class="nav--icons">
      <div class="news">
        <icon-base :icon-color="black"><icon-news /></icon-base>
      </div>
      <div class="notifications">
        <IconBase><IconNotifications /></IconBase>
      </div>
      <div class="messages">
        <IconBase><IconMessages /></IconBase>
      </div>
    </div>
    <div class="profile">
      <div class="profile--picture">
        <img src="../assets/Oghenetega.png" alt="Oghenetega" />
      </div>
      <div class="profile--name">
        Oghenetega
      </div>
      <div class="nav--dropdown">&#709;</div>
    </div>
  </div>
</template>

<script>
import IconBase from './IconBase';
import IconMessages from './icons/IconMessages';
import IconNews from './icons/IconNews';
import IconNotifications from './icons/IconNotifications';

export default {
  components: {
    IconMessages,
    IconNews,
    IconNotifications
  }
};
</script>

<style lang="scss" scoped>
.nav {
  display: grid;
  grid-template-columns: 2fr repeat(4, 1.5fr);
  grid-template-rows: 1fr;
  grid-column-gap: 0px;
  grid-row-gap: 0px;
  font-size: 1.6rem;
  padding: 0 5rem;

  div {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .profile {
    justify-content: space-between;

    &--picture {
      img {
        height: 10rem;
        width: 10rem;
      }
    }

    &--name {
      margin-right: auto;
    }
  }
}
</style>
