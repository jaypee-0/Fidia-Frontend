<template>
  <div class="row card rounded-lg border m-0 shadow-md mbottom width-32">
    <div class="d-flex justify-content-between w-100">
      <h5 class="fs-16">{{ dashboard.title }}</h5>
      <span
        >        
        <img src="../assets/svg-png-icons/3dots.png" alt="">        
      </span>
    </div>
    <div class="d-flex justify-content-between w-100 align-items-end">
      <div class="">
        <p class="fs-2 fw-bold">{{ dashboard.amount }}</p>
        <div class="d-flex textsm">
          <span>
            <svg
              version="1.1"
              id="Layer_1"
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              x="0px"
              y="0px"
              viewBox="0 0 483.284 483.284"
              style="enable-background: new 0 0 483.284 483.284"
              xml:space="preserve"
              width="20"
              class="arrow"
              height="15"
            >
              <polygon
                :style="
                  dashboard.per > dashboard.pre
                    ? dashboard.upColor
                    : dashboard.downColor
                "
                :points="
                  dashboard.per > dashboard.pre ? dashboard.up : dashboard.down
                "
              />
            </svg>
          </span>
          <p class="f-inter">{{ dashboard.per }}%</p>
          <span class="">vs last month</span>
        </div>
      </div>
      <div>
        <svg
          width="131"
          class="graph"
          height="76"
          viewBox="0 0 131 56"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <!-- gradient -->
          <path
            :d="
              dashboard.per > dashboard.pre
                ? dashboard.uptrendColor
                : dashboard.downtrendColor
            "
            :fill="
              dashboard.per > dashboard.pre
                ? 'url(#paint0_linear_2245_11831)'
                : 'url(#paint0_linear_2245_11813)'
            "
          />
          <path
            :d="
              dashboard.per > dashboard.pre
                ? dashboard.uptrend
                : dashboard.downtrend
            "
            :stroke="
              dashboard.per > dashboard.pre
                ? dashboard.uptrendStrokeColor
                : dashboard.downtrendStrokeColor
            "
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <defs>
            <linearGradient
              id="paint0_linear_2245_11813"
              x1="65.6667"
              y1="21"
              x2="65.6667"
              y2="62"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0" stop-color="red" stop-opacity="0" />
              <stop offset="1" stop-color="red" stop-opacity="0.3" />
            </linearGradient>
          </defs>

          <defs>
            <linearGradient
              id="paint0_linear_2245_11831"
              x1="65.3334"
              y1="1"
              x2="65.3334"
              y2="65"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0" stop-color="green" stop-opacity="0" />
              <stop offset="1" stop-color="green" stop-opacity="0.3" />
            </linearGradient>
          </defs>
        </svg>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["dashboard"],
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@500&display=swap");

.fs-2 {
  font-size: 32px;
}
.fs-16 {
  font-size: 16px;
  font-weight: 500;
}
.width-32 {
  width: 32%;
}
.fw-bold {
  font-weight: 600;
  line-height: 44px;
  font-style: normal;
  font-family: "Inter", sans-serif;
}
.f-inter {
  font-family: "Inter", sans-serif;
}
.graph {
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0) 64.12%,
    #ffffff 100%
  );
}
.card {
  padding: 24px 24px;
  flex-direction: row !important;
  border: unset;
}
@media (max-width: 320px) {
  .card {
    padding: 20px 16px;
  }
  .text {
    font-size: 30px;
    padding-top: 20px;
    padding-bottom: 16px;
  }
  .textsm {
    font-size: 14px;
  }
  .graph {
    width: 96px;
    height: 48px;
  }
  .arrow {
    width: 11px;
    height: 11px;
  }
  .width-32 {
  width: 100%;
  }
}
@media (max-width: 768px) {
  .width-32 {
  width: 100%;
  }
  .mbottom {
    margin-bottom: 0.8rem!important;
  }
}
</style>