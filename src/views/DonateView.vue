<template>
  <div class="donation">
    <div class="donationLeft">
      <div>
        Please Donate us,<br />
        Here is Our Bank Account
      </div>
    </div>
    <div class="DonationContainer">
      <div class="cardDonate">
        <div class="card__info">
          <div class="card__logo">CBGA ORGANIZATION</div>
          <div class="card__chip">
            <svg
              class="card__chip-lines"
              role="img"
              width="20px"
              height="20px"
              viewBox="0 0 100 100"
              aria-label="Chip"
            >
              <g opacity="0.8">
                <polyline
                  points="0,50 35,50"
                  fill="none"
                  stroke="#000"
                  stroke-width="2"
                />
                <polyline
                  points="0,20 20,20 35,35"
                  fill="none"
                  stroke="#000"
                  stroke-width="2"
                />
                <polyline
                  points="50,0 50,35"
                  fill="none"
                  stroke="#000"
                  stroke-width="2"
                />
                <polyline
                  points="65,35 80,20 100,20"
                  fill="none"
                  stroke="#000"
                  stroke-width="2"
                />
                <polyline
                  points="100,50 65,50"
                  fill="none"
                  stroke="#000"
                  stroke-width="2"
                />
                <polyline
                  points="35,35 65,35 65,65 35,65 35,35"
                  fill="none"
                  stroke="#000"
                  stroke-width="2"
                />
                <polyline
                  points="0,80 20,80 35,65"
                  fill="none"
                  stroke="#000"
                  stroke-width="2"
                />
                <polyline
                  points="50,100 50,65"
                  fill="none"
                  stroke="#000"
                  stroke-width="2"
                />
                <polyline
                  points="65,65 80,80 100,80"
                  fill="none"
                  stroke="#000"
                  stroke-width="2"
                />
              </g>
            </svg>
            <div class="card__chip-texture"></div>
          </div>
          <div class="card__type">CBE</div>
          <div class="card__number">
            <span class="card__digit-group">1000</span>
            <span class="card__digit-group">183</span>
            <span class="card__digit-group">802</span>
            <span class="card__digit-group">775</span>
          </div>
          <div class="card__valid-thru" aria-label="Valid thru">Valid for<br /></div>
          <div class="card__exp-date">
            <time datetime="2038-01"> 01/2022</time>
          </div>
          <div class="card__name" aria-label="Dee Stroyer">Hailemelekot Melakie</div>
          <div class="card__vendor" role="img" aria-labelledby="card-vendor">
            <span id="card-vendor" class="card__vendor-sr">Mastercard</span>
          </div>
        </div>
        <div class="card__texture"></div>
      </div>
    </div>
  </div>
</template>

<script>
import "@/css/donation.css";
export default {};
</script>
<style scoped>
.donation {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
}
.donationLeft {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
@media screen and (max-width: 890px) {
  .donation {
    flex-direction: column;
    padding: 5px;
  }
}
</style>
