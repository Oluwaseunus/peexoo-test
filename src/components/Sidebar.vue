<template>
  <div class="sidebar">
    <div class="logo"></div>
    <div class="links">
      <div class="link">
        <IconBase iconName="dashboard" iconColor="white"
          ><IconDashboard
        /></IconBase>
        Dashboard
      </div>
      <div class="link"><span class="icon icon--profile"></span> Profile</div>
      <div class="link">
        <span class="icon icon--package"></span> Pricing Package
      </div>
      <div class="link link--active">
        <span class="icon icon--availability"></span> Availability
      </div>
      <div class="link"><span class="icon icon--bookings"></span> Bookings</div>
      <div class="link">
        <span class="icon icon--portfolio"></span> Portfolio
      </div>
      <div class="link"><span class="icon icon--albums"></span> Albums</div>
      <div class="link">
        <span class="icon icon--subscriptions"></span> Subscriptions
      </div>
      <div class="link"><span class="icon icon--payments"></span> Payments</div>
      <div class="link"><span class="icon icon--settings"></span> Settings</div>
    </div>
    <div class="info">
      &copy; 2019 Peexoo Technologies
    </div>
  </div>
</template>

<script>
import IconBase from './IconBase';
import IconDashboard from './icons/IconDashboard';

export default {
  components: {
    IconBase,
    IconDashboard
  }
};
</script>

<style lang="scss" scoped>
.sidebar {
  background: #4d4d4d;
  padding: 2rem 0;
  color: #ccc;
  text-align: center;
  height: 100vh;

  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 1fr 5fr 1fr;
  grid-column-gap: 0px;
  grid-row-gap: 0px;
}

.logo {
  background: url('../assets/Asset 7.png');
  background-size: 85%;
  background-repeat: no-repeat;
  background-position: center;
  width: 85%;
  height: 8rem;
  margin: auto;
}

.links {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.link {
  font-size: 1.4rem;
  font-family: 'Montserrat', sans-serif;
  font-weight: 500;
  text-align: center;
  line-height: 17px;
  padding: 2rem 0;

  &--active {
    color: #ffb603;
    background: #5c5c5c;
    position: relative;

    &::before {
      content: '';
      height: 100%;
      width: 5%;
      position: absolute;
      left: 0;
      top: 0;
      background: #ffb603;
    }
  }

  .icon {
    fill: white;
  }
}

.info {
  font-size: 1.2rem;
  font-weight: 400;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
