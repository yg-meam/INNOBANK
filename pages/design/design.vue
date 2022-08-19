<template>
  <v-layout fill-height column>
    <div>
      <v-layout align-center class="my-2">
        <v-btn text class="ml-8 Innobank" width="200" @click="mainPage"
          >INNOBANK</v-btn
        >
        <v-btn text class="mr-8 design" width="80" @click="design"
          >디자인</v-btn
        >
        <v-spacer></v-spacer>
        <v-btn text class="mr-8 greyText" @click="Sintro">서비스소개</v-btn>
        <v-btn text class="mr-8 greyText">디자인 출원</v-btn>
        <v-btn text class="mr-8 greyText">등록디자인 검색</v-btn>
        <v-btn text class="mr-8 greyText">디자인특허 소식</v-btn>
        <v-btn text class="mr-8 greyText" @click="login"
          >로그인 / 회원가입</v-btn
        >
      </v-layout>
    </div>

    <v-card img="/img/write.jpg" height="600">
      <v-layout align-center justify-center style="height: 100%" column>
        <v-card-title style="height: 100%">
          <v-layout align-center justify-center column>
            <h2>당신의 디자인</h2>
            <h2>출원해서 보호받으세요.</h2>
            <h4>혁신을 믿고 맡길 수 있는, 이노뱅크</h4>
            <v-btn class="mt-10" rounded color="yellow" @click="application"
              >출원하기</v-btn
            >
          </v-layout>
        </v-card-title>
      </v-layout>
    </v-card>

    <v-card>
      <v-layout justify-center>
        <v-card-title class="mt-10">
          <v-layout column>
            <h5 class="orangText">절차안내</h5>
            <h5>쉽고 간편한</h5>
            <h5>서비스</h5>
            <v-row class="mt-10">
              <v-layout align-center column>
                <v-avatar color="orange" size="150">
                  <v-icon size="80" dark> mdi-account </v-icon>
                </v-avatar>
                <h5 class="mt-3">출원의뢰</h5>
              </v-layout>
              <v-icon class="ml-5" large> mdi-chevron-right</v-icon>
              <v-layout align-center column>
                <v-avatar class="ml-5" color="orange" size="150">
                  <v-icon size="80" dark> mdi-email </v-icon>
                </v-avatar>
                <h5 class="mt-3">출원서작성</h5>
              </v-layout>
              <v-icon class="ml-5" large> mdi-chevron-right</v-icon>
              <v-layout align-center column>
                <v-avatar class="ml-5" color="orange" size="150">
                  <v-icon size="80" dark> gavel </v-icon>
                </v-avatar>
                <h5 class="mt-3">심사</h5>
              </v-layout>
              <v-icon class="ml-5" large> mdi-chevron-right</v-icon>
              <v-layout align-center column>
                <v-avatar class="ml-5" color="orange" size="150">
                  <v-icon size="80" color="white">
                    mdi-arrow-up-bold-box-outline
                  </v-icon>
                </v-avatar>
                <h5 class="mt-3">등록&관리</h5>
              </v-layout>
            </v-row>
          </v-layout>
        </v-card-title>
      </v-layout>
      <v-layout justify-center column>
        <v-card-title class="mt-10">
          <v-layout align-center justify-center style="height: 100%">
            <h3>디자인출원 간편이용방법</h3>
          </v-layout>
        </v-card-title>
      </v-layout>
    </v-card>

    <v-card class="greyBackground" height="400">
      <v-layout justify-center>
        <v-card-title class="mt-10">
          <v-layout column>
            <h5 class="orangText">가격</h5>
            <h5>합리적인</h5>
            <h5>가격</h5>
            <v-row class="mt-5">
              <v-layout align-center justify-center column class="mr-15">
                <v-icon size="100"> tips_and_updates </v-icon>
                <v-card-title>
                  <v-layout align-center justify-center column>
                    <h4>15~25만원</h4>
                    <h5 class="greyText">출원수수료</h5>
                  </v-layout>
                </v-card-title>
              </v-layout>
              <v-layout align-center justify-center column class="mr-15">
                <v-icon size="100"> attach_money </v-icon>
                <v-card-title
                  ><v-layout align-center justify-center column>
                    <h4>0~20만원</h4>
                    <h5 class="greyText">중간사건 대응</h5>
                  </v-layout>
                </v-card-title>
              </v-layout>
              <v-layout align-center justify-center column>
                <v-icon size="100"> verified </v-icon>
                <v-card-title
                  ><v-layout align-center justify-center column>
                    <h4>15~25만원</h4>
                    <h5 class="greyText">등록/관리 수수료</h5>
                  </v-layout>
                </v-card-title>
              </v-layout>
            </v-row>
          </v-layout>
        </v-card-title>
      </v-layout>
    </v-card>

    <v-card class="black" height="200">
      <v-layout justify-center>
        <v-card-title class="mt-10 whiteText" style="height: 100%">
          <v-layout column>
            <h5>이노뱅크</h5>
            <h2 class="mt-5">나의 소중한 디자인,</h2>
            <h2>온라인으로 간편하게 출원해보세요.</h2>
          </v-layout>
          <v-btn class="ml-10" color="yellow">출원하러 가기</v-btn>
        </v-card-title>
      </v-layout>
    </v-card>

    <v-card height="500">
      <v-layout justify-center align-center style="height: 100%">
        <v-card-title style="height: 100%">
          <v-layout align-center justify-center column>
            <h5 class="orangText">궁금하신 질문 모아봤습니다.</h5>
            <h5>자주 묻는 질문</h5>
            <v-row>
              <v-card outlined class="mt-5" height="250" width="300">
                <v-card-title>
                  <h5>Q. 공인인증서 없이도 디자인 출원이 가능한가요?</h5>
                </v-card-title>
                <v-card-text>
                  <div>
                    네. 가능합니다. 저희 이노뱅크는 온라인으로 위임장을 작성해
                    드리며 복잡한 절차를 단순화 시켜드립니다.
                  </div>
                </v-card-text>
              </v-card>
              <v-card outlined class="mt-5 ml-5" height="250" width="300">
                <v-card-title>
                  <h5>Q. 나의 디자인이 출원전에 유출되진 않을까요?</h5>
                </v-card-title>
                <v-card-text>
                  <div>
                    이노뱅크 서비스는 고객님의 소중한 정보를 암호화된 SSL
                    프로토콜을 이용한 HTTPS 세션 네트워크를 통해 AWS서버에
                    전송되며, 미국 정부에서 채택된 암호화 방식을 통해
                    암호화하고, AWS 최고 수준의 보안 서버를 이용하여 인증정보를
                    관리하고 있습니다.
                  </div>
                </v-card-text>
              </v-card>
            </v-row>
          </v-layout>
        </v-card-title>
      </v-layout>
    </v-card>

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
    design() {
      this.$router.push("/design/design");
    },
    Sintro() {
      this.$router.push("/design/Sintro");
    },
    login() {
      this.$router.push("/login");
    },
    application() {},
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
.blackText {
  color: black;
}
.whiteText {
  color: white;
}
.orangText {
  color: darkorange;
}
.greyBackground {
  background-color: rgb(202, 202, 202);
}
.black {
  background-color: black;
}
.Innobank {
  font-weight: bold;
  font-size: 30px;
}
.design {
  font-size: 25px;
  color: orange;
}
</style>