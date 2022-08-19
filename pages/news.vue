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
        <v-btn text class="mr-8 blackText" @click="news">소식</v-btn>
        <v-btn text class="mr-8 greyText" @click="design">디자인</v-btn>
        <v-btn text class="mr-8 greyText" @click="login">로그인</v-btn>
      </v-layout>
    </div>

    <v-layout justify-center>
      <v-card-title class="mt-10">
        <v-layout column>
          <h1>특허소식</h1>
          <v-divider class="mt-10"></v-divider>

          <div v-for="(item, key) in list" :key="key">
            <v-row class="mt-5">
              <img :src="item.src" :href="item.link" width="100" height="100" />
              <v-layout column>
                <a :href="item.link" class="ml-5">{{ item.title }}</a>
                <v-card-text>{{ item.text }}</v-card-text>
              </v-layout>
            </v-row>
            <v-divider class="mt-5"></v-divider>
          </div>

          <div class="text-center">
            <v-pagination
              v-model="page"
              :length="2"
              @input="next"
            ></v-pagination>
          </div>
        </v-layout>
      </v-card-title>
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
    return {
      page: 1,
      list: [
        {
          title: "특허청 '스타트업 특허출원 지원해요' - 서울경제",
          link: "https://sedaily.com/NewsView/1VLVBVM1KX",
          src: "/img/startup.jpeg",
          text: "2019-07-28",
        },
        {
          title:
            "휴게소 먹방 아이콘 '소떡소떡' 특허 두고 中企 소송전 : 네이트뉴스",
          link: "https://m.news.nate.com/view/20190624n34995?sect=sisa&list=rank&cate=interest",
          src: "/img/food.webp",
          text: "2019-06-25",
        },
        {
          title: "[민후의 기·꼭·법] 등록하려는 디자인 모방, 처벌할 수 있을까?",
          link: "https://www.edaily.co.kr/news/read?newsId=01285766615992552&mediaCodeNo=257",
          src: "/img/minhu.jpeg",
          text: "2019-04-25",
        },
        {
          title:
            "[이데일리가 만났습니다] '최대3배 징벌적 배상, 특허침해 풍토바꾼다.' : 네이버 뉴스",
          link: "https://n.news.naver.com/mnews/article/018/0004328255?sid=101",
          src: "/img/daily.jpeg",
          text: "2019-03-31",
        },
        {
          title:
            "[오성환의 지식재산권이야기] '특허권 담보'대출 가능한가요? -Money S",
          link: "https://moneys.mt.co.kr/news/mwView.php?no=2019031311118082315&code=&MGSIN",
          src: "/img/property.jpeg",
          text: "2019-03-22",
        },
        {
          title: "특허청, 특허·영업비밀·디자인 침해 범죄 수사한다",
          link: "http://www.koscaj.com/news/articleView.html?idxno=111581",
          text: "2019-03-18",
        },
        {
          title:
            "[김종호의 특허TalK] 폴더블폰 다은은 롤러블폰?.. '폼 팩터' 경쟁치열 - 이데일리",
          link: "https://www.edaily.co.kr/news/read?newsId=01256246622419056&mediaCodeNo=257",
          src: "/img/phone.jpeg",
          text: "2019-03-01",
        },
        {
          title: "뷰티업계 '디자인은 곧 경쟁력' - 뷰티코리아뉴스",
          link: "http://www.bkn24.com/news/articleView.html?idxno=12137",
          src: "/img/perfume.png",
          text: "2019-02-22",
        },
        {
          title: "사업의 창과 방패가 되는 산업재산권 - AU경재 - 아유경제",
          link: "http://www.areyou.co.kr/news/articleView.html?idxno=41093",
          src: "/img/person.png",
          text: "2019-02-22",
        },
        {
          title:
            "[판결](단독) '디자인권 침해' 주장하며 법적절차 밟지 않고거래처에 경고장 발송은 - 법률신문",
          link: "https://m.lawtimes.co.kr/Content/Article?serial=150867",
          src: "/img/manga.png",
          text: "2019-02-21",
        },
        {
          title: "대표님, 왜 UX/UI를 출원하지 않으시나요?",
          link: "https://brunch.co.kr/@dawner/41",
          src: "/img/google.png",
          text: "2019-02-19",
        },
        {
          title: "애플 '폴더블 특허' 갱신... 삼성전자 의식? - 시사위크",
          link: "http://www.sisaweek.com/news/articleView.html?idxno=118524",
          src: "/img/apple.png",
          text: "2019-02-18",
        },
        {
          title:
            "대웅제약, 베아제 출시 33주년 맞아 새 TV 광고 선보여 - 이데일리",
          link: "https://www.edaily.co.kr/news/read?newsId=02378006622391832&mediaCodeNo=257",
          src: "/img/pill.png",
          text: "2019-02-18",
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
    news() {
      this.$router.push("/news");
    },
    service() {
      this.$router.push("/service");
    },
    privacy() {
      this.$router.push("/privacy");
    },
    next() {},
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
.blackText {
  color: black;
}
</style>