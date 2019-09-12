<template>
  <div class="sidebar">
    <div class="logo"></div>
    <div class="links">
      <div class="link">
        <IconBase iconName="Dashboard" iconColor="#fff"
          ><IconDashboard
        /></IconBase>
        <p class="link--text">
          Dashboard
        </p>
      </div>
      <div class="link">
        <IconBase iconName="Profile" iconColor="#fff"><IconProfile /></IconBase>
        <p class="link--text">
          Profile
        </p>
      </div>
      <div class="link">
        <IconBase iconName="Package" iconColor="#fff"><IconPackage /></IconBase>
        <p class="link--text">
          Pricing Package
        </p>
      </div>
      <div class="link link--active">
        <IconBase iconName="Availability" iconColor="#ffb603"
          ><IconAvailability
        /></IconBase>
        <p class="link--text">
          Availability
        </p>
      </div>
      <div class="link">
        <IconBase iconName="Bookings" iconColor="#fff"
          ><IconBookings
        /></IconBase>
        <p class="link--text">
          Bookings
        </p>
      </div>
      <div class="link">
        <IconBase iconName="Portfolio" iconColor="#fff"
          ><IconPortfolio
        /></IconBase>
        <p class="link--text">
          Portfolio
        </p>
      </div>
      <div class="link">
        <IconBase iconName="Albums" iconColor="#fff"><IconAlbums /></IconBase>
        <p class="link--text">
          Albums
        </p>
      </div>
      <div class="link">
        <IconBase iconName="Subscriptions" iconColor="#fff"
          ><IconSubscriptions
        /></IconBase>
        <p class="link--text">
          Subscriptions
        </p>
      </div>
      <div class="link">
        <IconBase iconName="Payments" iconColor="#fff"
          ><IconPayments
        /></IconBase>
        <p class="link--text">
          Payments
        </p>
      </div>
      <div class="link">
        <IconBase iconName="Settings" iconColor="#fff"
          ><IconSettings
        /></IconBase>
        <p class="link--text">
          Settings
        </p>
      </div>
    </div>
    <div class="info">
      &copy; 2019 Peexoo Technologies
    </div>
  </div>
</template>

<script>
import IconBase from './IconBase';
import IconAlbums from './icons/IconAlbums';
import IconAvailability from './icons/IconAvailability';
import IconBookings from './icons/IconBookings';
import IconDashboard from './icons/IconDashboard';
import IconPackage from './icons/IconPackage';
import IconPayments from './icons/IconPayments';
import IconPortfolio from './icons/IconPortfolio';
import IconProfile from './icons/IconProfile';
import IconSettings from './icons/IconSettings';
import IconSubscriptions from './icons/IconSubscriptions';

export default {
  components: {
    IconAlbums,
    IconAvailability,
    IconBase,
    IconBookings,
    IconDashboard,
    IconPackage,
    IconPayments,
    IconPortfolio,
    IconProfile,
    IconSettings,
    IconSubscriptions
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
  display: flex;
  justify-content: center;
  align-items: center;

  &--text {
    cursor: pointer;
  }

  &--active {
    color: #ffb603;
    background: #5c5c5c;
    position: relative;

    svg {
      fill: #ffb603;
    }

    &::before {
      content: '';
      height: 100%;
      width: 2%;
      position: absolute;
      left: 0;
      top: 0;
      background: #ffb603;
    }
  }

  .icon {
    fill: #fff;
  }
}

.info {
  font-size: 1.2rem;
  font-weight: 400;
  display: flex;
  justify-content: center;
  align-items: center;
}

svg {
  width: 1.8rem;
  height: 1.8rem;
  fill: #fff;
  margin-right: 1rem;
  margin-bottom: 0.2rem;
}
</style>
