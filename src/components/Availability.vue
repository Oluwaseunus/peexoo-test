<template>
  <div class="availability">
    <div class="header">
      <p class="title">Availability</p>
      <div class="switch--view">
        <div class="calendar--view">
          <!-- Calendar icon goes here -->
          Calendar view
        </div>
        <div class="list--view">
          <!-- List icon goes here -->
          List view
        </div>
      </div>
      <div class="search--schedule">
        <div class="searchbox">
          <input type="text" placeholder="Search" />
          <div class="search--button"></div>
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
  </div>
</template>

<style lang="scss" scoped>
.availability {
  padding: 6rem;
}

.header {
  position: relative;
  margin-bottom: 4rem;
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
  width: 20rem;
  justify-content: space-between;
  padding: 1rem 0;
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
  color: white;
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
    background: white;
    color: #ffb603;
    border: 1px solid #ffb603;
    padding: 0.6rem 1.7rem;
    text-transform: none;
  }
}

.searchbox {
  background: #fffefc;
  border: 1px solid #d4d4d4;
  border-radius: 1rem;
  justify-content: space-between;
  width: 23rem;
  position: relative;

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
