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

    <v-card height="600" img="/img/money.jpg">
      <v-layout align-center justify-center style="height: 100%">
        <v-card width="500" height="300">
          <v-card-title style="height: 100%">
            <v-layout align-center justify-center column>
              <h5>INNOBANK 상표서비스</h5>
              <h2>상표출원 선택이 아닌</h2>
              <h2>필수입니다.</h2>
              <v-card-text style="height: 100%">
                <v-layout align-center justify-center column>
                  <div>
                    - 우리나라 상표법은 먼저 출원한 자에게 권리를 부여합니다.
                  </div>
                  <div>
                    - 이 점을 악용한 국내외 브로커들이 활발히 활동하고 있습니다.
                  </div>
                  <div>
                    - 날이 갈수록 늘어나는 상표 분쟁으로부터 자유로워지려면,
                  </div>
                  <div>나의 브랜드를 빠르게 출원하는 것이 최선입니다.</div>
                </v-layout>
              </v-card-text>
            </v-layout>
          </v-card-title>
        </v-card>
      </v-layout>
    </v-card>

    <v-card color="black" height="200">
      <v-layout align-center justify-center style="height: 100%">
        <v-card-title class="whiteText" style="height: 100%">
          <v-layout align-center column>
            <h2>브랜드 네이밍부터 상표 출원까지</h2>
            <h2>전문가와 함께하세요.</h2>
          </v-layout>
        </v-card-title>
      </v-layout>
    </v-card>

    <v-card class="background2">
      <v-layout justify-center style="height: 100%">
        <v-card-title style="height: 100%">
          <v-layout justify-center align-center column>
            <h2>견적</h2>
            <h2>상담 요청하기</h2>
            <v-card-text style="height: 100%">
              <v-layout justify-center align-center column>
                <div>상담내용을</div>
                <div>간단하게 작성해주세요.</div>
              </v-layout>
            </v-card-text>
          </v-layout>
        </v-card-title>
        <div class="ml-10 mt-10">
          <v-text-field
            v-model="name"
            class="mb-2"
            hide-details
            label="작성자명"
            solo
            flat
            dense
          ></v-text-field>
          <v-text-field
            v-model="phone"
            class="mb-2"
            hide-details
            label="전화번호"
            solo
            flat
            dense
          ></v-text-field>
          <v-text-field
            v-model="password"
            type="password"
            class="mb-2"
            hide-details
            label="비밀번호"
            solo
            flat
            dense
          ></v-text-field>
          <v-textarea
            v-model="text"
            class="mb-2"
            hide-details
            :rows="3"
            auto-grow
            label="상담내용을 적어주세요"
            solo
            flat
            dense
          ></v-textarea>
          <v-btn class="mb-10" @click="consulting" outlined block
            >상담신청</v-btn
          >
        </div>
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
    return {
      name: "",
      phone: "",
      password: "",
      text: "",
    };
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
    consulting() {
      if (!this.name) {
        return window.alert("이름을 작성해주세요");
      } else if (!this.phone) {
        return window.alert("전화번호를 작성해주세요");
      } else if (!this.password) {
        return window.alert("비밀번호를 작성해주세요");
      } else {
        return window.alert("상담신청이 완료되었습니다");
      }
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
.whiteText {
  color: white;
}
.background2 {
  background-color: gainsboro;
}
</style>