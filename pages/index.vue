<template>
  <div class="">
    <div class="hero">
      <div class="welcome-box">
        <h1 class="welcome-text">Welcome Rob</h1>
        <v-btn
          color="white"
          class="welcome-btn welcome-btn-padding"
        >
          Change personal details
          <img class="welcome-btn-icon" :src="require('~/static/slidemenu.png')"/>
        </v-btn>
        <div class="welcome-image">
          <v-img :src="require('~/static/Table.png')"></v-img>
        </div>
      </div>
    </div>
    <div class="treatment-plan">
      <v-container>
        <v-row justify="center" align="center">
          <v-col cols="12" sm="12" md="8">
            <v-row justify="center" align="center">
              <v-col cols="12" sm="12" md="4">
                <img class="" :src="require('~/static/Image.png')"/>
              </v-col>
              <v-col cols="12" sm="12" md="8">
                <div class="d-flex">
                  <h2 class="title-text">Finasteride</h2> <span class="status">active</span>
                </div>
                <p class="description">For personalised advice, you are welcome to arrange a video consultation with a trained consultant or to use our live assistance for guidance while browsing online.</p>
                <div class="btn-box">
                  <v-row>
                    <v-col cols="12" sm="12" md="5">
                      <v-btn
                        color="white"
                        class="welcome-btn"
                      >
                        View treatment details
                        <img class="welcome-btn-icon" :src="require('~/static/arrow.png')"/>
                      </v-btn>
                    </v-col>
                    <v-col cols="12" sm="12" md="7">
                      <v-btn
                        color="white"
                        class="welcome-btn"
                      >
                        View treatment history
                        <img class="welcome-btn-icon" :src="require('~/static/slidemenu.png')"/>
                      </v-btn>
                    </v-col>
                  </v-row>
                </div>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="treatment-plan">
      <v-container>
        <v-row justify="center" align="center">
          <v-col cols="12" sm="12" md="8">
            <v-row justify="center" align="center">
              <v-col cols="12" sm="12" md="4">
                <img class="" :src="require('~/static/Image.png')"/>
              </v-col>
              <v-col cols="12" sm="12" md="8">
                <div class="d-flex">
                  <h2 class="title-text">Shampoo</h2> <span class="status">paid</span> <span class="status">delivered</span>
                </div>
                <p class="description">For personalised advice, you are welcome to arrange a video consultation with a trained consultant or to use our live assistance for guidance while browsing online.</p>
                <div class="btn-box">
                  <v-row>
                    <v-col cols="12" sm="12" md="5">
                      <v-btn
                        color="white"
                        class="welcome-btn"
                      >
                        View treatment details
                        <img class="welcome-btn-icon" :src="require('~/static/arrow.png')"/>
                      </v-btn>
                    </v-col>
                    <v-col cols="12" sm="12" md="7">
                      <v-btn
                        color="white"
                        class="welcome-btn"
                      >
                        View treatment history
                        <img class="welcome-btn-icon" :src="require('~/static/slidemenu.png')"/>
                      </v-btn>
                    </v-col>
                  </v-row>
                </div>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>
<style scoped lang="scss">
.v-btn--is-elevated{
  box-shadow: none;
}
.welcome-btn{
  margin-top: 30px;
  font-family: Inter;
  font-style: normal;
  font-weight: 600;
  font-size: 15px;
  text-transform: none;
  line-height: 27px;
  color: #2A2A2A;
  padding-top: 30px !important;
  padding-bottom: 30px !important;
  padding-left: 30px !important;
  border-radius: 0;
  border: 1px solid #e3e3e3 !important;
  .welcome-btn-icon{
    margin-left: 28px;
  }
}
.status{
  border: 0.5px solid #ACA7A7;
  box-sizing: border-box;
  border-radius: 1px;
  font-family: Inter;
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  height: 25px;
  padding-top: 3px;
  padding-left: 5px;
  padding-right: 5px;
  text-align: center;
  color: #092673;
  margin-top: 7px;
  margin-left: 20px;
}
.hero{
  .welcome-box{
    .welcome-btn-padding{
      margin-left: 145px;
    }
    .welcome-text{
      margin-left: 145px;
      margin-top: 183px;
      font-family: Inter;
      font-style: normal;
      font-weight: normal;
      font-size: 28px;
      line-height: 34px;
      color: #2A2A2A;
    }

    .welcome-image{
      margin-top: 30px;
    }
  }
}
.v-sheet.v-card:not(.v-sheet--outlined){
  box-shadow: none;
}
.treatment-plan{
  padding-top: 110px;
  padding-bottom: 110px;
  border-bottom: 2px solid #979797;
  box-sizing: border-box;
  .title-text{
    font-family: Inter;
    font-style: normal;
    font-weight: normal;
    font-size: 28px;
    line-height: 34px;
    color: #2A2A2A;
    margin-bottom: 20px;
  }
  .v-application p{
    margin-bottom: 0;
  }
  .description{
    font-family: Inter;
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 27px;
    color: #2A2A2A;
  }
}
@media (max-width: 480px) {
  .welcome-btn-padding {
    margin-left: 30px !important;
  }
  .welcome-text{
    margin-left: 30px !important;
  }
}
</style>
<script>
import Sparkline from "../components/Sparkline";
export default {
  components: {Sparkline}
}
</script>
