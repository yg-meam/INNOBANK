<template>
  <v-layout fill-height column>
    <div>
      <v-card height="60" class="overflow-hidden">
        <v-app-bar
          absolute
          color="white"
          elevate-on-scroll
          scroll-target="#scrolling-techniques-7"
        >
          <v-layout align-center class="my-2">
            <v-btn text class="ml-8 Innobank" width="200" @click="mainPage"
              >INNOBANK</v-btn
            >
            <v-btn text class="mr-8 design" width="80" @click="design"
              >디자인</v-btn
            >
            <v-spacer></v-spacer>
            <v-btn text class="mr-8 blackText" @click="Sintro"
              >서비스소개</v-btn
            >
            <v-btn text class="mr-8 greyText" @click="Deapp">디자인 출원</v-btn>
            <v-btn text class="mr-8 greyText">등록디자인 검색</v-btn>
            <v-btn text class="mr-8 greyText">디자인특허 소식</v-btn>
            <v-btn text class="mr-8 greyText" @click="login"
              >로그인 / 회원가입</v-btn
            >
          </v-layout>
        </v-app-bar>
        <v-sheet
          id="scrolling-techniques-7"
          class="overflow-y-auto"
          max-height="600"
        >
        </v-sheet>
      </v-card>
    </div>

    <v-layout justify-center style="height: 100%">
      <v-card-title class="mt-10" style="height: 100%">
        <v-layout column>
          <h5 class="orangText">출원절차</h5>
          <h5>간편하고 편리한</h5>
          <h5>디자인출원</h5>
          <v-row>
            <img class="mt-5" src="/img/consulting.jpg" height="250" />
            <v-card-title class="ml-10" style="height: 100%">
              <v-layout column>
                <h2>디자인출원,</h2>
                <h2>이노뱅크에 믿고 맡겨주세요.</h2>
                <v-card-text style="height: 100%">
                  <div>내 소중한 디자인, 남이 베끼게 내버려두시겠습니까?</div>
                  <div>
                    디자인 도용을 막는 유일한 방법은, 특허청에 디자인을 출원해서
                  </div>
                  <div>등록받는 것입니다.</div>
                  <div>
                    복잡하고 어려운 디자인 출원, 이노뱅크 변리사에게 믿고
                    맡겨주세요.
                  </div>
                </v-card-text>
              </v-layout>
            </v-card-title>
          </v-row>
        </v-layout>
      </v-card-title>
    </v-layout>
    <v-layout class="mt-10" justify-center style="height: 100%">
      <v-card-title class="mt-10" style="height: 100%">
        <v-row>
          <v-layout column>
            <h2>간편한 서비스</h2>
            <h2>합리적인 금액</h2>
            <v-card-text style="height: 100%">
              <div>
                온라인 간편 서비스를 통해 디장니 출원 비용을 합리적으로
                제공합니다.
              </div>
              <div>출원부터 등록까지 온라인으로 간편하게!</div>
              <div>이노뱅크에서 디자인의 가치를 보호하세요.</div>
            </v-card-text>
          </v-layout>
          <img class="ml-10 mb-10" src="/img/handshake.jpg" height="300" />
        </v-row>
      </v-card-title>
    </v-layout>

    <v-card class="mt-10" color="grey">
      <v-layout align-center>
        <div class="mt-5 mb-5 ml-16" @click="service">이용약관</div>
        <div class="ml-3 mr-3">·</div>
        <div @click="privacy">개인정보처리방침</div>
      </v-layout>
    </v-card>
    <v-card color="black">
      <div class="ml-16 pt-5 whiteText">
        특허법인이노뱅크 | 대표변리사 김태훈 김현석 윤원식 박기선 | 고객센터
        1644-1612 | 사업자등록번호 851-81-02176
      </div>
      <div class="ml-16 mt-2 pb-5 whiteText">
        통신판매업 2019-서울송파-1102 | 서울특별시 송파구 백제고분로 276,
        공익빌딩 502호
      </div>
    </v-card>
  </v-layout>
</template>

<script>
export default {
  data() {
    return {};
  },
  mounted() {},
  methods: {
    mainPage() {
      this.$router.push("/");
    },
    design() {
      this.$router.push("/design/design");
    },
    Sintro() {
      this.$router.push("/design/Sintro");
    },
    Deapp() {
      this.$router.push("/design/Deapp");
    },
    login() {
      this.$router.push("/login");
    },
    service() {
      this.$router.push("/service");
    },
    privacy() {
      this.$router.push("/privacy");
    },
  },
};
</script>

<style scoped>
.greyText {
  color: grey;
}
.blackText {
  color: black;
}
.Innobank {
  font-weight: bold;
  font-size: 30px;
}
.design {
  font-size: 25px;
  color: orange;
}
.orangText {
  color: darkorange;
}
.whiteText {
  color: white;
}
</style>