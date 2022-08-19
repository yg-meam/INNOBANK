<template>
  <v-layout fill-height column>
    <div>
      <v-layout align-center>
        <img src="/img/bulb.jpg" style="width: 60px" class="ml-8" />
        <div class="mr-5" @click="mainPage">INNOBANK</div>
        <img src="/img/telephone.jpg" style="width: 60px" />
        <div class="phoneNumber">1644-1612</div>
        <v-spacer></v-spacer>
        <v-btn text class="mr-8 greyText" @click="introduce">회사소개</v-btn>
        <v-btn text class="mr-8 greyText" @click="work">업무영역</v-btn>
        <v-btn text class="mr-8 greyText" @click="consulting">무료상담</v-btn>
        <v-btn text class="mr-8 greyText" color="gray">소식</v-btn>
        <v-btn text class="mr-8 greyText" @click="design">디자인</v-btn>
        <v-btn text class="mr-8 greyText" @click="login">로그인</v-btn>
      </v-layout>
    </div>

    <v-layout class="background pb-10" align-center justify-center column>
      <div class="people">
        <div class="mt-15">INNOBANK</div>
        <div>구성원 소개</div>
      </div>
      <img src="/img/person4.png" height="500" width="400" />
      <v-layout>
        <img
          class="rounded-circle mt-5 mr-5"
          src="/img/Bperson1.png"
          onmouseover="this.src='/img/person1.png';"
          onmouseout="this.src='/img/Bperson1.png';"
          @click="kimtaehoon"
          height="80"
          width="80"
        />
        <img
          class="rounded-circle mt-5 mr-5"
          src="/img/Bperson2.png"
          onmouseover="this.src='/img/person2.png';"
          onmouseout="this.src='/img/Bperson2.png';"
          @click="kimhyunseok"
          height="80"
          width="80"
        />
        <img
          class="rounded-circle mt-5 mr-5"
          src="/img/Bperson3.png"
          onmouseover="this.src='/img/person3.png';"
          onmouseout="this.src='/img/Bperson3.png';"
          @click="parkkisun"
          height="80"
          width="80"
        />
        <img
          class="rounded-circle mt-5 mr-5"
          src="/img/person4.png"
          @click="yunwonsig"
          height="80"
          width="80"
        />
        <img
          class="rounded-circle mt-5 mr-5"
          src="/img/Bperson5.png"
          onmouseover="this.src='/img/person5.png';"
          onmouseout="this.src='/img/Bperson5.png';"
          @click="yangchanghoon"
          height="80"
          width="80"
        />
        <img
          class="rounded-circle mt-5 mr-5"
          src="/img/Bperson6.png"
          onmouseover="this.src='/img/person6.png';"
          onmouseout="this.src='/img/Bperson6.png';"
          @click="ryuhongcheol"
          height="80"
          width="80"
        />
      </v-layout>
      <v-card class="background" flat height="500" width="500">
        <v-layout align-center justify-center column style="height: 100%">
          <v-card-title style="height: 100%">
            <v-layout align-center justify-center column>
              <h5>특허법인 이노뱅크</h5>
              <h1>윤원식</h1>

              <v-card-text class="mt-5" style="height: 100%">
                <v-layout align-center justify-center column>
                  <h3>EDUCATION</h3>
                  <div>- 2011 한양대학교 응용화학과 졸업</div>
                  <div>- 2019 고려대학교 공학대학원 지식재산학과 석사</div>
                  <h3 class="mt-5">CAREER</h3>
                  <div>- 현 특허법인 이노뱅크 대표 변리사 (2019~)</div>
                  <div>- 현 신제품(NEP) 인증 심사위원</div>
                  <div>- 현 중소벤처기업부 비지니스지원단 클리닉 위원</div>
                  <div>- 현 조달청 우수조달제품 심사위원</div>
                  <div>- 현 한국특허전략개발원 표준특허 전문변리사</div>
                  <div>- 현 경기과학기술진흥원 기술지원사업 평가위원</div>
                  <div>- 현 시흥산업진흥원 기술장인</div>
                  <div>- 현 경기테크노파크 전문인력</div>
                  <div>- 전 특허법인 청운 변리사</div>
                  <div>- 전 21세기 특허법률사무소 변리사</div>
                  <div>- 전 특허법인 세림 변리사</div>
                  <div>- 전 도울국제특허법률사무소 대표 변리사</div>
                </v-layout>
              </v-card-text>
            </v-layout>
          </v-card-title>
        </v-layout>
      </v-card>
    </v-layout>

    <v-card color="grey">
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
    introduce() {
      this.$router.push("/introduce");
    },
    work() {
      this.$router.push("/work");
    },
    consulting() {
      this.$router.push("/consulting");
    },
    design() {
      this.$router.push("/design/design");
    },
    login() {
      this.$router.push("/login");
    },
    kimtaehoon() {
      this.$router.push("/attorney/kimtaehoon");
    },
    kimhyunseok() {
      this.$router.push("/attorney/kimhyunseok");
    },
    parkkisun() {
      this.$router.push("/attorney/parkkisun");
    },
    yunwonsig() {
      this.$router.push("/attorney/yunwonsig");
    },
    yangchanghoon() {
      this.$router.push("/attorney/yangchanghoon");
    },
    ryuhongcheol() {
      this.$router.push("/attorney/ryuhongcheol");
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
.phoneNumber {
  color: red;
}
.greyText {
  color: grey;
}
.people {
  font-weight: bold;
  font-size: 40px;
}
.whiteText {
  color: white;
}
.background {
  background-color: #eee;
}
</style>