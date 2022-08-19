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
        <v-btn text class="mr-8 blackText" @click="work">업무영역</v-btn>
        <v-btn text class="mr-8 greyText" @click="consulting">무료상담</v-btn>
        <v-btn text class="mr-8 greyText">소식</v-btn>
        <v-btn text class="mr-8 greyText" @click="design">디자인</v-btn>
        <v-btn text class="mr-8 greyText" @click="login">로그인</v-btn>
      </v-layout>
    </div>

    <v-card img="/img/building.jpg" height="600">
      <v-layout align-center justify-center style="height: 100%">
        <v-card width="500" height="300">
          <v-card-title style="height: 100%">
            <v-layout align-center justify-center column>
              <h2>We Make Innovation to worth</h2>
              <v-card-text class="mt-5 pb-10">
                <v-layout align-center justify-center column>
                  <div>
                    귀사의 소중한 발명을 가치 있는 지식재산권으로 만들어
                    드립니다.
                  </div>
                  <div>
                    또한, 확보된 지식재산권을 활용하여 성공의 디딤돌이 되도록
                  </div>
                  <div>최선을 다하겠습니다.</div>
                </v-layout>
              </v-card-text>
              <v-btn outlined @click="download">회사소개서 보기</v-btn>
            </v-layout>
          </v-card-title>
        </v-card>
      </v-layout>
    </v-card>

    <v-card height="400">
      <v-layout justify-center align-center style="height: 100%">
        <v-card-title style="height: 100%" class="mr-10">
          <v-layout align-center justify-center column>
            <h3>TOTAL SERVICE</h3>
            <v-card-text style="height: 100%">
              <v-layout align-center justify-center column>
                <div>지식재산 토탈 서비스 제공</div>
              </v-layout>
            </v-card-text>
          </v-layout>
        </v-card-title>
        <v-avatar color="orange" size="200">
          <v-layout align-center justify-center column>
            <h4>IP</h4>
            <h4>서비스</h4>
          </v-layout>
        </v-avatar>
        <v-avatar size="200">
          <v-layout align-center justify-center column>
            <h4>특허관리</h4>
            <h4>프로그램</h4>
          </v-layout>
        </v-avatar>
        <v-avatar color="orange" size="200">
          <v-layout align-center justify-center column>
            <h4>지식재산권 교육</h4>
            <h4>& 컨설팅</h4>
          </v-layout>
        </v-avatar>
      </v-layout>
    </v-card>

    <v-card class="greyBackground" height="700">
      <v-layout justify-center align-center style="height: 100%">
        <v-card-title style="height: 100%" class="mr-10">
          <v-layout align-center justify-center column>
            <h3>QUALITY&SPEED</h3>
            <v-card-text style="height: 100%">
              <v-layout align-center justify-center>
                <div>최상의 품질과 빠른 속도</div>
              </v-layout>
            </v-card-text>
          </v-layout>
        </v-card-title>
        <div class="mr-5">
          <v-card height="300" width="250" class="mb-5">
            <v-card-title>
              <v-layout column>
                <h5>최상·균일 품질 관리</h5>
                <h5>변리사 직접 작성</h5>
              </v-layout>
            </v-card-title>
            <v-card-text>
              <v-layout column>
                <div>· 이노뱅크는 변리사가 직접 명세서를 작성합니다.</div>
                <div>
                  · 출원 명세서, 의견서/보정서 등 모든 대응 서류를 빠르고
                  확실하게 처리합니다.
                </div>
                <div>
                  · 이노뱅크의 변리사는 모두 파트너 변리사로 책임감을 가지고
                  업무를 수행합니다.
                </div>
                <div class="pt-4 greyText">IP SERVICE</div>
              </v-layout>
            </v-card-text>
          </v-card>
          <v-card height="250" width="250">
            <v-card-title>
              <v-layout column>
                <h5>내용관련</h5>
              </v-layout>
            </v-card-title>
            <v-card-text>
              <v-layout column>
                <div>
                  · 명세서 작성시 복수의 변리사가 검수하여 퀄리티를 유지합니다.
                </div>
                <div>· 가장 넓은 권리범위를 확보할 수 있도록 고민합니다.</div>
                <div>· 불필요한 중간사건이 발생하지 않도록 노력합니다.</div>
                <div class="pt-4 greyText">IP SERVICE</div>
              </v-layout>
            </v-card-text>
          </v-card>
        </div>
        <div>
          <v-card height="250" width="250" class="mb-5">
            <v-card-title>
              <v-layout column>
                <h5>절차관련</h5>
              </v-layout>
            </v-card-title>
            <v-card-text>
              <v-layout column>
                <div>· 기일을 철저하게 지킵니다.</div>
                <div>· 기간연장을 최소화합니다.</div>
                <div>
                  · 자체 프로그램을 통해서 정확하고 안전하게 관리합니다.
                </div>
                <div class="pt-15 greyText">IP SERVICE</div>
              </v-layout>
            </v-card-text>
          </v-card>
          <v-card height="300" width="250">
            <v-card-title>
              <v-layout column>
                <h5>신속·간편하고</h5>
                <h5>합리적인 금액</h5>
              </v-layout>
            </v-card-title>
            <v-card-text>
              <v-layout column>
                <div>· 출원 비용을 합리적으로 제공합니다.</div>
                <div>
                  · 출원인의 요청에 따라 최대한 빠른 출원을 약속드립니다.
                </div>
                <div>· 온라인 서비스를 통해 비대면 출원 의뢰가 가능합니다.</div>
                <div class="pt-15 greyText">IP SERVICE</div>
              </v-layout>
            </v-card-text>
          </v-card>
        </div>
      </v-layout>
    </v-card>

    <v-card height="600">
      <v-layout justify-center align-center style="height: 100%">
        <v-card-title style="height: 100%" class="mr-10">
          <v-layout align-center justify-center column>
            <h3>IP SERVICE</h3>
            <v-card-text style="height: 100%">
              <v-layout align-center justify-center column>
                <div>이노뱅크만의 특별한</div>
                <div>IP 서비스</div>
              </v-layout>
            </v-card-text>
          </v-layout>
        </v-card-title>
        <div class="mr-5">
          <v-card height="220" width="250" class="mb-5">
            <v-card-title>
              <v-layout column>
                <h5>IP 창출</h5>
              </v-layout>
            </v-card-title>
            <v-card-text>
              <v-layout column>
                <div>· 아이디어 상담 및 출원 전략 수립</div>
                <div>· 선행기술 조사, 특허동향조사</div>
                <div>· R&D 전략 기획</div>
                <div>· 상표 상담 및 브랜드 개발</div>
                <div class="pt-8 greyText">IP SERVICE</div>
              </v-layout>
            </v-card-text>
          </v-card>
          <v-card height="220" width="250">
            <v-card-title>
              <v-layout column>
                <h5>IP 권리화</h5>
              </v-layout>
            </v-card-title>
            <v-card-text>
              <v-layout column>
                <div>
                  · 국내 IP(특허/실용신안/상표/디자인)의 출원부터 등록까지
                </div>
                <div>· 특허료 및 등록연치료 관리</div>
                <div class="pt-14 greyText">IP SERVICE</div>
              </v-layout>
            </v-card-text>
          </v-card>
        </div>
        <div>
          <v-card height="220" width="250" class="mb-5">
            <v-card-title>
              <v-layout column>
                <h5>IP 보호</h5>
              </v-layout>
            </v-card-title>
            <v-card-text>
              <v-layout column>
                <div>· 무효심판, 취소심판 심결취소소송</div>
                <div>· 경고장 및 답변서 작성</div>
                <div>· 침해소송, 가처분신청, 손해배당</div>
                <div>· 권리 침해 판단 및 감정서 작성</div>
                <div class="pt-8 greyText">IP SERVICE</div>
              </v-layout>
            </v-card-text>
          </v-card>
          <v-card height="220" width="250">
            <v-card-title>
              <v-layout column>
                <h5>IP 활용</h5>
              </v-layout>
            </v-card-title>
            <v-card-text>
              <v-layout column>
                <div>· IP 담보대출 상담</div>
                <div>· 가지급금, 이익잉여금 처리</div>
                <div>· IP 가치평가 및 거래</div>
                <div>· IP 실시권 설정</div>
                <div class="pt-8 greyText">IP SERVICE</div>
              </v-layout>
            </v-card-text>
          </v-card>
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
    download() {
      window.open("https://innobank.co.kr/download/innobank_KOR.pdf");
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
.blackText {
  color: black;
}
.greyText {
  color: grey;
}
.phoneNumber {
  color: red;
}
.greyBackground {
  background-color: rgb(202, 202, 202);
}
.grey {
  background-color: gray;
}
.whiteText {
  color: white;
}
</style>
