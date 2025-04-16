<div class="team">
  <p class="team-title">Team</p>
  <div style:padding-top="35px" style:padding-bottom="35px">
      <div class="team-portraits" >
          <div class="portrait-background aron">
              <div class="portrait-image" style:width="300px" style:height="300px" style:background-image="url('/webp/aron.webp')"></div>
              <div class="portrait-text">Aron</div>
          </div>
          <div class="portrait-background zimran">
              <div class="portrait-image" style:width="300px" style:height="300px" style:background-image="url('/webp/zimran.webp')"></div>
              <div class="portrait-text">Zimran</div>
          </div>
          <div class="portrait-background evik">
              <div class="portrait-image" style:width="260px" style:height="260px" style:background-image="url('/webp/evik.webp')"></div>
              <div class="portrait-text">evik</div>
          </div>
          <div class="portrait-background reka">
              <div class="portrait-image" style:width="244px" style:height="244px" style:background-image="url('/webp/reka.webp')"></div>
              <div class="portrait-text">Reka</div>
          </div>
          <div class="portrait-background anna">
              <div class="portrait-image" style:width="284px" style:height="284px" style:background-image="url('/webp/anna.webp')"></div>
              <div class="portrait-text">Anna</div>
          </div>
          <div class="portrait-background mate">
              <div class="portrait-image" style:width="281px" style:height="281px" style:background-image="url('/webp/mate.webp')"></div>
              <div class="portrait-text">Mate</div>
          </div>
          <div class="portrait-background timi">
              <div class="portrait-image" style:width="276px" style:height="276px" style:background-image="url('/webp/timi.webp')"></div>
              <div class="portrait-text">Timi</div>
          </div>
          <div class="portrait-background sanyi">
              <div class="portrait-image" style:width="308px" style:height="308px" style:background-image="url('/webp/sanyi.webp')"></div>
              <div class="portrait-text">Sanyi</div>
          </div>
      </div>
  </div>
</div>


<style>
.team-portraits{
  height: 2000px;
  margin-left:-450px;
}

.aron {
  width: 352px;
  height: 417px;
  transform: rotate(12deg);
  top: 0;
  left: 274px;
  z-index: 1;
  font-size: 48px;
}

.evik {
  width: 305px;
  height: 361px;
  transform: rotate(6deg);
  top: -12px;
  left: 546px;
  z-index: 0;
}

.reka {
  width: 287px;
  height: 341px;
  transform: rotate(-12deg);
  top: -340px;
  left: 171px;
  z-index: 0;
}

.anna {
  width: 334px;
  height: 396px;
  transform: rotate(0.1deg);
  top: -320px;
  left: 480px;
  z-index: 1;
}

.mate {
  width: 331px;
  height: 392px;
  transform: rotate(10deg);
  top: -640px;
  left: 133px;
  z-index: 0;
}

.timi {
  width: 324px;
  height: 384px;
  transform: rotate(-19deg);
  top: -460px;
  left: 250px;
  z-index: 1;
}

.sanyi {
  width: 362px;
  height: 429px;
  top: -1040px;
  left: 495px;
  z-index: 0;
}

.portrait-background {
  background-color: #fff;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  position: relative;
  filter: drop-shadow(10px 10px 6px rgba(0, 0, 0, 0.7));
}

.portrait-image {
  background-position: center;
  margin: 0 auto 10px auto;
}

.team {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: column;
}

.team-title {
  font-family: "OldNewspaperTypes";
  font-style: normal;
  font-weight: 500;
  font-size: 64px;
  text-align: center;
  color: #fff;
  margin-bottom: 100px;
}

.portrait-text {
  font-family: "FuzzyBubbles";
  font-weight: 400;
  font-size: 40px;
  text-align: center;
  color: #000;
  margin: 0 auto;
}

/*MOBILE*/
@media (max-width: 850px) {
  .team-portraits {
    transform: scale(0.5);
    margin-left:-300px;
    margin-top: -420px;
    height: 1350px;
  }

  .team {
    padding-top:10px;
  }
}


@media(max-width: 440px){
  .team-portraits {
    height: 1200px;
    transform: scale(0.3);
    margin-left:-200px;
    margin-top: -450px;
    margin-bottom: -180px;
  }

  .portrait-image {
    width:246px !important;
    height:236px !important;
  }

  .team-title {
    margin-bottom: 20px;
    font-size: 48px;
  }
}
</style>


