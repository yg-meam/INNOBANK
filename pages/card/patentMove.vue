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

    <v-card height="600" img="/img/people.jpg">
      <v-layout align-center justify-center style="height: 100%">
        <v-card width="500" height="300">
          <v-card-title style="height: 100%">
            <v-layout align-center justify-center column>
              <h5>INNOBANK 특허서비스</h5>
              <h2>전담 변리사 제도 도입</h2>
              <v-card-text style="height: 100%">
                <v-layout align-center justify-center column>
                  <div>대부분의 특허사무소는 상담만 변리사가 진행하고,</div>
                  <div>실제 일처리는 직원이나 수습 변리사들이 수행합니다.</div>
                  <div>
                    문제는, 담당자가 퇴사하게 될 경우에는 업무의 팔로우가 전혀
                    되지
                  </div>
                  <div>않는다는 것입니다.</div>
                  <div>
                    이노뱅크는 출원부터 등록까지 한 명의 전담 변리사가 끝까지
                    관리합니다.
                  </div>
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
          <v-layout column>
            <h2>발명의 대략적인 컨셉을 적어주시면,</h2>
            <h2>전담 변리사를 매칭해드립니다.</h2>
          </v-layout>
          <v-row>
            <v-card-text class="ml-10" style="height: 100%">
              <v-layout column>
                <h3>변리사법 제23조(도용 및 누설의 죄)</h3>
                <div>
                  변리사이거나 변리사였던 사람이 정당한 사유 없이 업무상 알게 된
                  발명자, 고안자,
                </div>
                <div>
                  창작자, 특허출원인 또는 실용시안·디자인등록출원인의 발명, 고안
                  또는 창작의 비밀을
                </div>
                <div>
                  누설(漏泄)하거나 도용(盜用)하였을 때에는 5년 이하의 징역 또는
                  5천만원 이하의 벌금에 처한다.
                </div>
                <div>'개정 2013.7.30., 2017.3.27.'</div>
              </v-layout>
            </v-card-text>
          </v-row>
        </v-card-title>
      </v-layout>
    </v-card>

    <v-card class="background2">
      <v-layout justify-center style="height: 100%">
        <v-card-title style="height: 100%">
          <v-layout justify-center align-center column>
            <h2>변리사</h2>
            <h2>매칭신청</h2>
            <v-card-text style="height: 100%">
              <v-layout justify-center align-center column>
                <div>특허 아이디어를</div>
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
            label="아이디어 컨셉"
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