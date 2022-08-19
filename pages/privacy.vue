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

    <v-layout class="background2" column>
      <v-layout class="mt-10 mb-10" justify-center>
        <h1>개인정보의 수집 이용목적</h1>
      </v-layout>
      <v-layout justify-center column class="mb-10">
        <v-layout column class="ml-5 mb-10">
          <h2>1. 개인정보의 수집 이용목적</h2>
          <h4>
            ① 이노뱅크(innobank.co.kr)은 다음과 같은 목적을 위하여 개인정보를
            수집하고 있습니다.
          </h4>
          <div>
            - 서비스제공을 위한 계약의 성립(본인식별 및 본인의사 확인 등)
          </div>
          <div>- 서비스의 이행(서비스제공 및 대금결제)</div>
          <div>- 기타 새로운 서비스, 신상품이나 이벤트 정보 안내</div>
          <h4>
            ② 단, 이용자의 기본적 인권 침해의 우려가 있는 민감한 개인정보(인종
            및 민족, 사상 및 신조, 출신지 및 본적지, 정치적 성향 및 범죄기록,
            건강상태 및 성생활 등)는 수집하지 않습니다.
          </h4>
          <v-layout column class="mt-10">
            <h2>2. 수집하는 개인정보의 항목</h2>
            <div>
              - 개인 회원: 이름, 생년월일, 비밀번호, 우편물 수령 주소,
              주민등록상 주소, 전화번호, 이동전화, 팩스번호, 이메일 주소, 우편물
              주소
            </div>
            <div>
              - 국내법인 회원: 법인명, 대표이사 이름, 법인번호, 사업자번호,
              우편물 수령 주소, 법인등록상 주소, 담당자 이름, 전화번호,
              이동전화, 팩스번호, 이메일 주소
            </div>
          </v-layout>
          <v-layout column class="mt-10">
            <h2>3. 개인정보의 보유 및 이용 기간</h2>
            <h4>
              ① 귀하의 개인정보는 다음과 같이 개인정보의 수집목적 또는 제공받은
              목적이 달성되면 파기됩니다.
            </h4>
            <div>
              - 신청서 작성한 경우, 신청의 철회 대리인변경을 통한 계약만료될
              때까지 보유
            </div>
            <div>
              - 대금지급정보의 경우, 대금의 완제일 또는 채권소멸시효기간의
              만료될 때까지 보유
            </div>
            <div>
              - 배송정보의 경우, 물품 또는 서비스가 인도되거나 제공될 때까지
              보유
            </div>
            <div>
              - 지적재산권업무 위임정보의 경우, 대리인의 선임을
              이노뱅크(innobank.co.kr) 혹은 이노뱅크의 제휴특허법률사무소가 아닌
              다른 대리인을 선임하고 이를 이노뱅크에 통지될 때까지 보유
            </div>
            <div>
              (단, 상법 등 법령의 규정에 의하여 보존할 필요성이 있는 경우에는
              예외로 함)
            </div>
          </v-layout>
        </v-layout>
      </v-layout>
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
.background2 {
  background-color: gainsboro;
}
.phoneNumber {
  color: red;
}
.whiteText {
  color: white;
}
.greyText {
  color: grey;
}
</style>