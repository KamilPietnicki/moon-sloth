<template>
  <div class="main">
    <div class="info-grid">
      <div class="text">
        <h1 class="title">MOON SLOTH TOKENOMICS</h1>
        <p>
          Moon Sloth is a community-based project fully built for the community
          and proud to be the first project raccoon-based project to aim and
          land on the moon in the upcoming months. <br />
          Our token functions are simple yet effective at deflating the total
          supply of $MoonSloth while allowing it to gain attraction and
          momentum.
        </p>
      </div>
      <div class="stats">
        <h2>7% <br> TOTAL <br> TAX</h2>
        <h2>2% <br> ADDED <br> LIQUIDITY</h2>
        <h2>2% <br> INSTANT <br> REWARDS</h2>
        <h2>3% <br> TRANSACTION <br> LIMIT</h2>
      </div>
      <div class="text"></div>
      <div class="images"></div>
    </div>

    <div class="box">
            <ul id="first-list">
                <li>
                    <span></span>
                    <div class="title">INITIAL GOALS</div>
                    <br>
                    <div class="info"> - 100 Telegram Group Members</div>
                    <div class="info"> - 100 Telegram Group Members</div>
                    <div class="info"> - 100 Telegram Group Members</div>
                    <div class="info"> - 100 Telegram Group Members</div>

                    <div class="time">
                        <span>STEP 1</span>
                        <span></span>
                    </div>
                </li>
                <li>
                    <span></span>
                    <div class="title">LAUNCH</div>
                    <br>
                    <div class="info"> - 100 Telegram Group Members</div>
                    <div class="info"> - 100 Telegram Group Members</div>
                    <div class="info"> - 100 Telegram Group Members</div>
                    <div class="info"> - 100 Telegram Group Members</div>

                    <div class="time">
                        <span>STEP 2</span>
                        <span></span>
                    </div>
                </li>
                <li>
                    <span></span>
                    <div class="title">POST-LAUNCH</div>
                    <br>
                    <div class="info"> - 100 Telegram Group Members</div>
                    <div class="info"> - 100 Telegram Group Members</div>
                    <div class="info"> - 100 Telegram Group Members</div>
                    <div class="info"> - 100 Telegram Group Members</div>
                    <div class="time">
                        <span>STEP 3</span>
                        <span></span>
                    </div>
                </li>
            </ul>
        </div>
  </div>
</template>

<script>
export default {
  components: {},
};
</script>

<style lang="scss">
.main {
  display: block;
  position: relative;

  width: 100%;
  height: auto;
}

.info-grid {
  display: grid;
  position: relative;

  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  gap: 20px;

  .stats {
    display: grid;
    position: relative;

    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr 1fr;

    place-items: center;
    text-align: center;
    
  }
}

.box{
    margin:0 10%;
    height: 630px;
    overflow: hidden;
    padding: 10px 0 40px 60px
}

.box ul{
    list-style-type: none;
    margin: 0;
    padding: 0;
    position: relative;
    transition: all 0.5s linear;
    top:0
}

.box ul:last-of-type{top:80px}

.box ul:before{
    content: "";
    display: block;
    width: 0;
    height: 100%;
    border:1px dashed #ff6d6d;
    position: absolute;
    top:0;
    left:30px
}

.box ul li{
    margin: 20px 60px 60px;
    position: relative;
    padding: 10px 20px;
    background:rgba(255, 255, 255, 0.3);
    border-radius: 10px;
    line-height: 20px;
    width: 35%
}


.box ul li > span{
    content: "";
    display: block;
    width: 0;
    height: 100%;
    border:1px solid #ff6d6d;
    position: absolute;
    top:0;
    left:-30px
}

.box ul li > span:before,.box ul li > span:after{
    content: "";
    display: block;
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background:#ff6d6d;
    border:2px solid #ff6d6d;
    position: absolute;
    left:-5px
}

.box ul li > span:before{top:-10px}
.box ul li > span:after{top:95%}

.box .title{
    text-transform: uppercase;
    font-size: 24px;
    font-weight: 700;
    margin-bottom: 5px
}

.box .info:first-letter{text-transform: capitalize;line-height: 1.7}

.box .name{
    margin-top: 10px;
    text-transform: capitalize;
    font-style: italic;
    text-align: right;
    margin-right: 20px
}


.box .time span{
    position: absolute;
    left: -100px;
    font-size:80%;
    font-weight: bold;
}
.box .time span:first-child{top:-16px}
.box .time span:last-child{top:94%}
</style>