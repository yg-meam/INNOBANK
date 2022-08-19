<template>
  <v-layout fill-height column>
    <div>
      <v-layout align-center>
        <img src="/img/bulb.jpg" style="width: 60px" class="ml-8" />
        <div class="mr-5" @click="mainPage">INNOBANK</div>
        <img src="/img/telephone.jpg" style="width: 60px" />
        <div class="phoneNumber">1644-1612</div>
        <v-spacer></v-spacer>
        <v-btn text class="mr-8 blackText" @click="introduce">회사소개</v-btn>
        <v-btn text class="mr-8 greyText" @click="work">업무영역</v-btn>
        <v-btn text class="mr-8 greyText" @click="consulting">무료상담</v-btn>
        <v-btn text class="mr-8 greyText" color="gray">소식</v-btn>
        <v-btn text class="mr-8 greyText" @click="design">디자인</v-btn>
        <v-btn text class="mr-8 greyText" @click="login">로그인</v-btn>
      </v-layout>
    </div>

    <v-card img="/img/technology.jpg" height="600">
      <v-layout justify-center align-center style="height: 100%">
        <v-card width="500" height="300">
          <div fill-height style="height: 100%">
            <v-card-title style="height: 100%">
              <v-layout justify-center align-center column>
                <h2>Who is INNOBANK</h2>
                <v-card-text class="mt-5">
                  <v-layout justify-center align-center column>
                    <div>- 젊고 유능한 전문인력으로 구성된 거품없는 사무소</div>
                    <div>
                      - 합리적인 비용으로 업무 처리와 불필요한 비용발생 최소화
                    </div>
                    <div>
                      - 삼성, LG, 네이버 등 대기업, 중소기업, 스타트업까지 담당
                      경력
                    </div>
                    <div>- 10년 이상 경력의 변리사가 운영하는 특허법인</div>
                    <div>- 기업의 입장에서 생각할 줄 아는 변리사</div>
                  </v-layout>
                </v-card-text>
              </v-layout>
            </v-card-title>
          </div>
        </v-card>
      </v-layout>
    </v-card>

    <v-card>
      <v-layout justify-center>
        <v-card-title>
          <v-layout align-center justify-center column>
            <h3>OUR</h3>
            <h3>CLIENT</h3>
            <v-card-text>
              <v-layout align-center justify-center column>
                <div>고객사의 이익을 위해 세계적 수준의 기술을 보호하는</div>
                <div>이노뱅크의 경쟁력은 탁월합니다.</div>
                <div>고객사의 유기적인 상호 협력으로 함께 성장, 발전하는</div>
                <div>윈윈 전략을 실천합니다.</div>
              </v-layout>
            </v-card-text>
          </v-layout>
        </v-card-title>
        <div class="mr-5 mt-10 mb-10">
          <div>
            <img
              class="mb-2"
              src="/img/Bkolmar.png"
              onmouseover="this.src='/img/Kolmar.png';"
              onmouseout="this.src='/img/Bkolmar.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bbio.png"
              onmouseover="this.src='/img/Bio.png';"
              onmouseout="this.src='/img/Bbio.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bmagenta.jpeg"
              onmouseover="this.src='/img/Magenta.jpeg';"
              onmouseout="this.src='/img/Bmagenta.jpeg';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bkangnam.png"
              onmouseover="this.src='/img/Kangnam.png';"
              onmouseout="this.src='/img/Bkangnam.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bonda.png"
              onmouseover="this.src='/img/Onda.png';"
              onmouseout="this.src='/img/Bonda.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              src="/img/Bmjc.jpeg"
              onmouseover="this.src='/img/Mjc.jpeg';"
              onmouseout="this.src='/img/Bmjc.jpeg';"
              height="50"
              width="100"
            />
          </div>
        </div>
        <div class="mr-5 mt-10 mb-10">
          <div>
            <img
              class="mb-2"
              src="/img/Bkolmar.png"
              onmouseover="this.src='/img/Kolmar.png';"
              onmouseout="this.src='/img/Bkolmar.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bbio.png"
              onmouseover="this.src='/img/Bio.png';"
              onmouseout="this.src='/img/Bbio.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bmagenta.jpeg"
              onmouseover="this.src='/img/Magenta.jpeg';"
              onmouseout="this.src='/img/Bmagenta.jpeg';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bkangnam.png"
              onmouseover="this.src='/img/Kangnam.png';"
              onmouseout="this.src='/img/Bkangnam.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bonda.png"
              onmouseover="this.src='/img/Onda.png';"
              onmouseout="this.src='/img/Bonda.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              src="/img/Bmjc.jpeg"
              onmouseover="this.src='/img/Mjc.jpeg';"
              onmouseout="this.src='/img/Bmjc.jpeg';"
              height="50"
              width="100"
            />
          </div>
        </div>
        <div class="mr-5 mt-10 mb-10">
          <div>
            <img
              class="mb-2"
              src="/img/Bkolmar.png"
              onmouseover="this.src='/img/Kolmar.png';"
              onmouseout="this.src='/img/Bkolmar.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bbio.png"
              onmouseover="this.src='/img/Bio.png';"
              onmouseout="this.src='/img/Bbio.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bmagenta.jpeg"
              onmouseover="this.src='/img/Magenta.jpeg';"
              onmouseout="this.src='/img/Bmagenta.jpeg';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bkangnam.png"
              onmouseover="this.src='/img/Kangnam.png';"
              onmouseout="this.src='/img/Bkangnam.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bonda.png"
              onmouseover="this.src='/img/Onda.png';"
              onmouseout="this.src='/img/Bonda.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              src="/img/Bmjc.jpeg"
              onmouseover="this.src='/img/Mjc.jpeg';"
              onmouseout="this.src='/img/Bmjc.jpeg';"
              height="50"
              width="100"
            />
          </div>
        </div>
        <div class="mr-5 mt-10 mb-10">
          <div>
            <img
              class="mb-2"
              src="/img/Bkolmar.png"
              onmouseover="this.src='/img/Kolmar.png';"
              onmouseout="this.src='/img/Bkolmar.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bbio.png"
              onmouseover="this.src='/img/Bio.png';"
              onmouseout="this.src='/img/Bbio.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bmagenta.jpeg"
              onmouseover="this.src='/img/Magenta.jpeg';"
              onmouseout="this.src='/img/Bmagenta.jpeg';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bkangnam.png"
              onmouseover="this.src='/img/Kangnam.png';"
              onmouseout="this.src='/img/Bkangnam.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              class="mb-2"
              src="/img/Bonda.png"
              onmouseover="this.src='/img/Onda.png';"
              onmouseout="this.src='/img/Bonda.png';"
              height="50"
              width="100"
            />
          </div>
          <div>
            <img
              src="/img/Bmjc.jpeg"
              onmouseover="this.src='/img/Mjc.jpeg';"
              onmouseout="this.src='/img/Bmjc.jpeg';"
              height="50"
              width="100"
            />
          </div>
        </div>
      </v-layout>
    </v-card>
    <v-card class="greyBackground">
      <v-layout justify-center>
        <v-card-title class="mr-15">
          <v-layout align-center justify-center column>
            <h3>OUR</h3>
            <h3>HISTORY</h3>
            <v-card-text>
              <v-layout align-center justify-center column>
                <div>이노뱅크는 눈에 보이는 실적 그 이상의</div>
                <div>가치를 생각합니다.</div>
                <div>고객님과의 신뢰를 바탕으로 가치를 높이기 위해 꾸준히</div>
                <div>노력하고 있습니다.</div>
              </v-layout>
            </v-card-text>
          </v-layout>
        </v-card-title>
        <v-timeline>
          <v-timeline-item
            v-for="(year, i) in years"
            :key="i"
            color="orange"
            small
          >
            <template v-slot:opposite>
              <span
                :class="`headline font-weight-bold`"
                v-text="year.year"
              ></span>
            </template>
            <div class="py-4">
              <div style="white-space: pre-line" v-text="year.text"></div>
            </div>
          </v-timeline-item>
        </v-timeline>
      </v-layout>
    </v-card>

    <v-card class="pb-10">
      <v-layout justify-center>
        <v-layout align-center justify-center column>
          <v-card-title class="mt-14">
            <v-layout align-center justify-center column>
              <h2>TEAM</h2>
              <h2>MEMBER</h2>
            </v-layout>
          </v-card-title>
          <v-slide-group
            v-model="model"
            class="pa-4"
            active-class="success"
            show-arrows
          >
            <v-slide-item v-for="(photo, n) in photos" :key="n">
              <v-card class="ma-4" height="430" width="200">
                <v-layout align-center column>
                  <img :src="photo.src" width="200" height="300" />
                  <h3>{{ photo.name }}</h3>
                  <div>
                    {{ photo.ment }}
                  </div>
                  <v-btn class="mt-5" outlined @click="movePage(photo)"
                    >자세히 보기</v-btn
                  >
                </v-layout>
              </v-card>
            </v-slide-item>
          </v-slide-group>
        </v-layout>
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
      model: null,
      years: [
        {
          year: "2019.04",
          text: "이노뱅크 특허법률사무소 개소\n 디자인 출원 전문 플랫폼 'INNOBANK'개설 및 운영\n 경상북도 농업 기술원 전담사무소 선정 ",
        },
        {
          year: "2019.05",
          text: "미국, 중국, 일본, 유럽, 싱가포르 등 해외 특허법인과 업무 협약 체결",
        },
        {
          year: "2020.01",
          text: "한국콜마 주식회사 전담 사무소 선정",
        },
        {
          year: "2020.02",
          text: "윤원식 변리사, 박기선 변리사 영입 총 변리사 4인으로 사무소 확장이전\n KMA한국 능률 협회 스타트업 전담 사무소 선정",
        },
        {
          year: "2021.01",
          text: "양창훈 변리사, 류홍철 변리사 영입",
        },
        {
          year: "2021.03",
          text: "특허법인 이노뱅크 설립",
        },
      ],
      photos: [
        {
          src: "/img/person1.png",
          name: "김태훈",
          ment: "이노뱅크 변리사",
          text: "kimtaehoon",
        },
        {
          src: "/img/person2.png",
          name: "김현석",
          ment: "이노뱅크 변리사",
          text: "kimhyunseok",
        },
        {
          src: "/img/person3.png",
          name: "박기선",
          ment: "이노뱅크 변리사",
          text: "parkkisun",
        },
        {
          src: "/img/person4.png",
          name: "윤원식",
          ment: "이노뱅크 변리사",
          text: "yunwonsig",
        },
        {
          src: "/img/person5.png",
          name: "양창훈",
          ment: "이노뱅크 변리사",
          text: "yangchanghoon",
        },
        {
          src: "/img/person6.png",
          name: "류홍철",
          ment: "이노뱅크 변리사",
          text: "ryuhongcheol",
        },
      ],
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
    changePhoto() {},
    movePage(photo) {
      this.$router.push("/attorney/" + photo.text);
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
.whiteText {
  color: white;
}
</style>
