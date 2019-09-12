<template>
  <div class="calendar">
    <div class="days">
      <div class="day">
        <span>Sun</span>
      </div>
      <div class="day">
        <span>Mon</span>
      </div>
      <div class="day">
        <span>Tue</span>
      </div>
      <div class="day">
        <span>Wed</span>
      </div>
      <div class="day">
        <span>Thur</span>
      </div>
      <div class="day">
        <span>Fri</span>
      </div>
      <div class="day">
        <span>Sat</span>
      </div>
    </div>
    <div class="weeks">
      <div class="week">
        <div class="day weekday">
          <span>1</span>
        </div>
        <div class="day weekday booked">
          <span>2</span>
          <div class="event">
            <p>Mrs. Steven daughter’s wedding photography</p>
          </div>
        </div>
        <div class="day weekday">
          <span>3</span>
        </div>
        <div class="day weekday">
          <span>4</span>
        </div>
        <div class="day weekday">
          <span>5</span>
        </div>
        <div class="day weekday">
          <span>6</span>
        </div>
        <div class="day weekday">
          <span>7</span>
        </div>
      </div>
      <div class="week">
        <div class="day weekday">
          <span>8</span>
        </div>
        <div class="day weekday">
          <span>9</span>
        </div>
        <div class="day weekday">
          <span>10</span>
        </div>
        <div class="day weekday booked booked--group">
          <div class="booked--days">
            <span>11</span>
            <span>12</span>
            <span>13</span>
          </div>
          <div class="event">
            <p>Mrs. Peter daughter’s wedding photography</p>
          </div>
        </div>
        <div class="day weekday">
          <span>14</span>
        </div>
      </div>
      <div class="week">
        <div class="day weekday">
          <span>15</span>
        </div>
        <div class="day weekday ">
          <span>16</span>
        </div>
        <div class="day weekday">
          <span>17</span>
        </div>
        <div class="day weekday">
          <span>18</span>
        </div>
        <div class="day weekday">
          <span>19</span>
        </div>
        <div class="day weekday">
          <span>20</span>
        </div>
        <div class="day weekday">
          <span>21</span>
        </div>
      </div>
      <div class="week">
        <div class="day weekday">
          <span>22</span>
        </div>
        <div class="day weekday ">
          <span>23</span>
        </div>
        <div class="day weekday">
          <span>24</span>
        </div>
        <div class="day weekday">
          <span>25</span>
        </div>
        <div class="day weekday">
          <span>26</span>
        </div>
        <div class="day weekday">
          <span>27</span>
        </div>
        <div class="day weekday booked">
          <span>28</span>
          <div class="event">
            <p>Mrs. Steven daughter’s wedding photography</p>
          </div>
        </div>
      </div>
      <div class="week">
        <div class="day weekday">
          <span>29</span>
        </div>
        <div class="day weekday ">
          <span>30</span>
        </div>
        <div class="day weekday">
          <span></span>
        </div>
        <div class="day weekday">
          <span></span>
        </div>
        <div class="day weekday">
          <span></span>
        </div>
        <div class="day weekday">
          <span></span>
        </div>
        <div class="day weekday">
          <span></span>
        </div>
      </div>
    </div>
  </div>
</template>

<script></script>

<style lang="scss" scoped>
.days,
.week {
  display: flex;
  width: 100%;
  justify-content: space-between;
}

.day {
  font-family: 'Montserrat', sans-serif;
  font-size: 1.2rem;
  line-height: 1.4rem;
  text-transform: uppercase;
  flex: 1;

  display: flex;
  justify-content: center;
  align-items: center;
  border: 1px solid #d4d4d4;
  border-radius: 0.3rem;
  height: 5rem;
  background: #fff;
}

.weekday {
  height: 12.5rem;
}

.booked {
  background-color: #fff3d4;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;

  &--days {
    width: 100%;
    display: flex;
    justify-content: space-evenly;
  }

  &--group {
    flex-grow: 3;

    .event {
      text-align: center;
    }
  }
}

.event {
  background-color: #ffb603;
  width: 80%;
  padding: 1rem;
  text-transform: none;
  color: #fff;
}
</style>
