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
        <v-btn text class="mr-8 greyText" @click="news">소식</v-btn>
        <v-btn text class="mr-8 greyText" @click="design">디자인</v-btn>
        <v-btn text class="mr-8 greyText" @click="login">로그인</v-btn>
      </v-layout>
    </div>

    <!-- <no-ssr>
      <swiper class="swiper" :options="swiperOption">
        <div
          class="parallax-bg"
          slot="parallax-bg"
          data-swiper-parallax="-23%"
        ></div>
        <swiper-slide>
          <div class="title" data-swiper-parallax="-100">Slide 1</div>
          <div class="subtitle" data-swiper-parallax="-240">Subtitle</div>
          <div class="text" data-swiper-parallax="-360">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam
              dictum mattis velit, sit amet faucibus felis iaculis nec. Nulla
              laoreet justo vitae porttitor porttitor. Suspendisse in sem justo.
              Integer laoreet magna nec elit suscipit, ac laoreet nibh euismod.
              Aliquam hendrerit lorem at elit facilisis rutrum. Ut at
              ullamcorper velit. Nulla ligula nisi, imperdiet ut lacinia nec,
              tincidunt ut libero. Aenean feugiat non eros quis feugiat.
            </p>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="title" data-swiper-parallax="-100">Slide 2</div>
          <div class="subtitle" data-swiper-parallax="-240">Subtitle</div>
          <div class="text" data-swiper-parallax="-360">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam
              dictum mattis velit, sit amet faucibus felis iaculis nec. Nulla
              laoreet justo vitae porttitor porttitor. Suspendisse in sem justo.
              Integer laoreet magna nec elit suscipit, ac laoreet nibh euismod.
              Aliquam hendrerit lorem at elit facilisis rutrum. Ut at
              ullamcorper velit. Nulla ligula nisi, imperdiet ut lacinia nec,
              tincidunt ut libero. Aenean feugiat non eros quis feugiat.
            </p>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="title" data-swiper-parallax="-100">Slide 3</div>
          <div class="subtitle" data-swiper-parallax="-240">Subtitle</div>
          <div class="text" data-swiper-parallax="-360">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam
              dictum mattis velit, sit amet faucibus felis iaculis nec. Nulla
              laoreet justo vitae porttitor porttitor. Suspendisse in sem justo.
              Integer laoreet magna nec elit suscipit, ac laoreet nibh euismod.
              Aliquam hendrerit lorem at elit facilisis rutrum. Ut at
              ullamcorper velit. Nulla ligula nisi, imperdiet ut lacinia nec,
              tincidunt ut libero. Aenean feugiat non eros quis feugiat.
            </p>
          </div>
        </swiper-slide>
        <div
          class="swiper-pagination swiper-pagination-white"
          slot="pagination"
        ></div>
        <div
          class="swiper-button-prev swiper-button-white"
          slot="button-prev"
        ></div>
        <div
          class="swiper-button-next swiper-button-white"
          slot="button-next"
        ></div>
      </swiper>
    </no-ssr> -->
    <v-carousel
      cycle
      hide-delimiter-background
      :show-arrows="false"
      height="600"
    >
      <v-carousel-item v-for="(item, i) in items" :key="i" :src="item.src">
      </v-carousel-item>
    </v-carousel>

    <v-card class="background">
      <v-layout justify-center>
        <v-card width="300" height="200" class="mr-3">
          <div fill-height style="height: 100%">
            <v-card-title style="height: 100%">
              <v-layout align-center justify-center>
                <h3>특허출원</h3>
              </v-layout>
              <v-card-text>
                <v-layout align-center justify-center>
                  혁신적인 아이디어를 보호합니다.
                </v-layout>
              </v-card-text>
              <v-layout align-center justify-center>
                <v-btn width="50" @click="patentMove">바로가기</v-btn>
              </v-layout>
            </v-card-title>
          </div>
        </v-card>

        <v-card width="300" height="200" class="mr-3">
          <div fill-height style="height: 100%">
            <v-card-title style="height: 100%">
              <v-layout align-center justify-center>
                <h3>상표출원</h3>
              </v-layout>
              <v-card-text>
                <v-layout align-center justify-center>
                  브랜드의 가치를 지킵니다.
                </v-layout>
              </v-card-text>
              <v-layout align-center justify-center>
                <v-btn width="50" @click="brandMove">바로가기</v-btn>
              </v-layout>
            </v-card-title>
          </div>
        </v-card>

        <v-card width="300" height="200" class="mr-3">
          <div fill-height style="height: 100%">
            <v-card-title style="height: 100%">
              <v-layout align-center justify-center>
                <h3>디자인출원</h3>
              </v-layout>
              <v-card-text>
                <v-layout align-center justify-center>
                  제품의 외관을 보호합니다.
                </v-layout>
              </v-card-text>
              <v-layout align-center justify-center>
                <v-btn width="50" @click="patentMove">바로가기</v-btn>
              </v-layout>
            </v-card-title>
          </div>
        </v-card>
      </v-layout>

      <v-layout justify-center class="mb-10">
        <v-card-title class="mt-14 mr-10">
          <v-layout align-center justify-center column>
            <h3>언제나 친절한 무료 상담 서비스</h3>
            <h3>(1644-1614)</h3>
            <v-card-text>
              <v-layout align-center justify-center column>
                <div>
                  지식재산과 관련된 문제가 발생할 경우, 언제든지 연락주세요.
                </div>
                <div>전문 분야별로 변리사가 직접 상담해드립니다.</div>
              </v-layout>
            </v-card-text>
            <v-card-title class="mt-5 mr-10">
              <v-layout align-center justify-center column>
                <h3>지식재산 전문가 집단</h3>
                <v-card-text>
                  <v-layout align-center justify-center column>
                    <div>
                      이노뱅크는 지식재산의 출원부터 심판, 소송, 기술평가 등
                      다양한 업무를 수행하고 있습니다.
                    </div>
                    <div>
                      대형 로펌에서의 근무 경험을 바탕으로 탄탄한 기본기와
                    </div>
                    <div>문제 해결 능력을 갖춘 변리사들이 모였습니다.</div>
                    <div>
                      대한민국에서 가장 일 잘하는 전문가 집단 이노뱅크를 믿고
                      맡겨주세요.
                    </div>
                  </v-layout>
                </v-card-text>
              </v-layout>
            </v-card-title>
            <v-card-title class="mt-5 mr-10">
              <v-layout align-center justify-center column>
                <h3>스타트업, 중소기업 맞춤형 서비스</h3>
                <v-card-text>
                  <v-layout align-center justify-center column>
                    <div>
                      이노뱅크는 스타트업, 중소기업을 가장 잘 알고 있는
                      특허법인입니다.
                    </div>
                    <div>
                      아이디어와 고도화, 지식재산의 창출, 특허 매입 등을 통해서
                      회사의 가치를
                    </div>
                    <div>한층 더 업그레이드해 드립니다.</div>
                    <div>또한, 이노뱅크만의 고객 관리 서비스를 통해서</div>
                    <div>
                      지역/규모/업력 등에 따라 지식재산 지원 사업을
                      안내해드립니다.
                    </div>
                  </v-layout>
                </v-card-text>
              </v-layout>
            </v-card-title>
          </v-layout>
        </v-card-title>

        <img src="/img/book.jpg" width="300" height="700" class="mt-14" />
      </v-layout>
    </v-card>

    <v-card>
      <v-layout justify-center>
        <v-layout align-center justify-center column>
          <v-card-title class="mt-14">
            <h2>파트너 변리사</h2>
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
      <v-layout class="mt-16 mb-16" justify-center>
        <v-card-title class="mr-10">
          <v-layout align-center justify-center column>
            <h2>최첨단 시스템</h2>
            <h2>이노뱅크</h2>
            <v-card-text class="mt-5">
              <v-layout justify-center align-center column>
                <div>자체 특허관리 시스템을 통해,</div>
                <div>내 지식재산권 관리를 한눈에!</div>
              </v-layout>
            </v-card-text>
          </v-layout>
        </v-card-title>
        <img class="mt-16 mb-16" src="/img/tab.jpg" width="600" height="400" />
      </v-layout>

      <v-card class="background2">
        <v-layout justify-center>
          <v-card-title class="mt-16">
            <v-layout justify-center align-center column>
              <h2>무료</h2>
              <h2>상담신청</h2>
              <v-card-text class="mt-5">
                <v-layout justify-center align-center column>
                  <div>부담스러웠던 상담신청</div>
                  <div>간편하게 신청해서 상담하세요.</div>
                </v-layout>
              </v-card-text>
            </v-layout>
          </v-card-title>
          <div class="ml-10">
            <v-select
              v-model="kind"
              class="mt-10 mb-2"
              hide-details
              :items="categorys"
              label="카테고리"
              solo
              flat
            ></v-select>
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
              label="상담내용을 적어주세요."
              solo
              flat
              dense
            ></v-textarea>
            <v-btn class="mb-10" @click="application" outlined block
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
    </v-card>
  </v-layout>
</template>

<script>
export default {
  // name: "swiper-example-parallax",
  // title: "Parallax",

  data() {
    return {
      // swiperOption: {
      //   speed: 600,
      //   parallax: true,
      //   pagination: {
      //     el: ".swiper-pagination",
      //     clickable: true,
      //   },
      //   navigation: {
      //     nextEl: ".swiper-button-next",
      //     prevEl: ".swiper-button-prev",
      //   },
      // },
      model: null,
      kind: null,
      name: "",
      phone: "",
      password: "",
      text: "",
      items: [
        {
          src: "/img/write.jpg",
        },
        {
          src: "/img/people.jpg",
        },
        {
          src: "/img/technology.jpg",
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
      categorys: [
        { text: "특허/실용신안", value: "patent" },
        { text: "상표권", value: "brand" },
        { text: "디자인권", value: "design" },
        { text: "저작권", value: "copyright" },
        { text: "기타", value: "etc" },
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
    patentMove() {
      this.$router.push("/card/patentMove");
    },
    brandMove() {
      this.$router.push("/card/brandMove");
    },
    movePage(photo) {
      this.$router.push("/attorney/" + photo.text);
    },
    application() {
      if (this.kind == null) {
        return window.alert("카테고리를 선택해주세요");
      } else if (!this.name) {
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
    news() {
      this.$router.push("/news");
    },
  },
};
</script>

<style scoped>
.background {
  background-color: rgb(254, 255, 247);
}
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
/* parallax-bg {
   position: absolute;
   left: 0;
   top: 0;
   width: 130%;
   height: 100%;
   background-size: cover;
   background-position: left;
   background-image: url("/images/example/1.jpg");
 }

 .swiper {
   width: 100%;
   height: 380px;

   .swiper-slide {
     display: flex;
     flex-direction: column;
     justify-content: center;

     box-sizing: border-box;
     padding: 0 80px;
    background-color: transparent;

     .title {
       font-weight: bold;
     }

     .subtitle {
     }

   .text {
      max-width: 430px;
       line-height: 1.32;
     }
   }
 } */
</style>