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
        <IconBase iconName="News" iconColor="#4D4D4D"><IconNews /></IconBase>
      </div>
      <div class="notifications">
        <IconBase iconName="Notifications" iconColor="#4D4D4D"
          ><IconNotifications
        /></IconBase>
      </div>
      <div class="messages">
        <IconBase iconName="Messages" iconColor="#4D4D4D"
          ><IconMessages
        /></IconBase>
      </div>
    </div>
    <div class="profile">
      <img
        src="../assets/Oghenetega.png"
        alt="Oghenetega"
        class="profile--picture"
      />
      <div class="profile--name">
        Oghenetega
      </div>
      <div class="nav--dropdown">
        <IconBase iconName="ArrowDown" iconColor="black"
          ><IconArrowDown
        /></IconBase>
      </div>
    </div>
  </div>
</template>

<script>
import IconBase from './IconBase';
import IconArrowDown from './icons/IconArrowDown';
import IconMessages from './icons/IconMessages';
import IconNews from './icons/IconNews';
import IconNotifications from './icons/IconNotifications';

export default {
  components: {
    IconArrowDown,
    IconBase,
    IconMessages,
    IconNews,
    IconNotifications
  }
};
</script>

<style lang="scss" scoped>
.nav {
  display: grid;
  grid-template-columns: 4fr repeat(2, 1fr) 0.65fr 1.4fr;
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
      height: 10rem;
      width: 10rem;
    }
  }

  & > &--icons {
    display: flex;
    justify-content: space-evenly;
  }

  svg {
    cursor: pointer;
  }
}
</style>
