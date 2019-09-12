<template>
  <div class="availability">
    <div class="header">
      <p class="title">Availability</p>
      <div class="switch--view">
        <div class="calendar--view">
          <IconBase iconName="Calendar" iconColor="#B58000">
            <IconAvailability />
          </IconBase>
          Calendar view
        </div>
        <div class="list--view">
          <IconBase iconName="List" iconColor="#B58000">
            <IconList />
          </IconBase>
          List view
        </div>
      </div>
      <div class="search--schedule">
        <div class="searchbox">
          <input type="text" placeholder="Search" />
          <IconBase iconName="Search" iconColor="#D4D4D4">
            <IconSearch />
          </IconBase>
        </div>
        <button class="btn">+ Add Schedule</button>
      </div>
    </div>

    <div class="current--month">
      <div class="current--month__arrows">
        <div class="arrow previous--month">
          &#x25C4;
        </div>

        <div class="arrow next--month">
          &#x25BA;
        </div>
      </div>

      <p>September 2019</p>

      <button class="btn btn--inverted">Today</button>
    </div>
    <Calendar />
  </div>
</template>

<script>
import Calendar from './Calendar';
import IconBase from './IconBase';
import IconAvailability from './icons/IconAvailability';
import IconList from './icons/IconList';
import IconSearch from './icons/IconSearch';

export default {
  components: {
    Calendar,
    IconBase,
    IconAvailability,
    IconList,
    IconSearch
  }
};
</script>

<style lang="scss" scoped>
.availability {
  padding: 6rem;
}

.header {
  position: relative;
}

.title {
  font-size: 2.4rem;
  font-weight: 700;
  line-height: 2.9rem;
  color: #4d4d4d;
  font-family: 'Lora', sans-serif;
}

.switch--view {
  font-family: 'Montserrat', sans-serif;
  color: #b58000;
  font-weight: 400;
  font-size: 1.4rem;
  line-height: 1.9rem;
  display: flex;
  width: 22rem;
  justify-content: space-between;
  padding: 1rem 0;
  cursor: pointer;

  svg {
    margin-bottom: 0.4rem;
  }
}

.search--schedule {
  display: flex;
  justify-content: space-between;
  position: absolute;
  width: 40rem;
  right: 0;
  top: 2rem;
}

.btn {
  color: #fff;
  text-transform: uppercase;
  font-size: 1.4rem;
  font-weight: 500;
  font-family: 'Montserrat', sans-serif;
  line-height: 1.7rem;
  text-align: center;
  background: #ffb603;
  box-shadow: none;
  margin: 0;
  padding: 1rem 1.2rem;
  border: none;
  border-radius: 1rem;
  cursor: pointer;

  &:active,
  &:focus {
    outline: none;
  }

  &--inverted {
    background: #fff;
    color: #ffb603;
    border: 1px solid #ffb603;
    padding: 0.6rem 1.7rem;
    text-transform: none;
  }
}

.searchbox {
  background: #fffefc;
  border: 1px solid #d4d4d4;
  border-radius: 0.4rem;
  justify-content: space-between;
  width: 23rem;
  position: relative;

  svg {
    position: absolute;
    top: 0.7rem;
    right: 1rem;
  }

  input {
    border: none;
    height: 2.8rem;
    width: 18rem;
    position: absolute;
    top: 0.4rem;
    left: 1.5rem;

    &:focus {
      outline: none;
    }
  }
}

.current--month {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 25%;
  font-size: 1.8rem;
  margin: 2rem 0;

  &__arrows {
    display: flex;
  }

  p {
    color: #4d4d4d;
  }
}

.arrow {
  font-size: 1.8rem;
  cursor: pointer;
}
</style>
