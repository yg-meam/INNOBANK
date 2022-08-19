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
        <v-btn text class="mr-8 blackText" @click="consulting">무료상담</v-btn>
        <v-btn text class="mr-8 greyText" color="gray">소식</v-btn>
        <v-btn text class="mr-8 greyText" @click="design">디자인</v-btn>
        <v-btn text class="mr-8 greyText" @click="login">로그인</v-btn>
      </v-layout>
    </div>

    <v-card img="/img/meeting.jpg" height="600">
      <v-layout justify-center align-center style="height: 100%">
        <v-card width="500" height="300">
          <v-card-title style="height: 100%">
            <v-layout align-center justify-center column>
              <h2>무료</h2>
              <h2>상담신청</h2>
              <v-card-text style="height: 100%" class="mb-5">
                <v-layout align-center justify-center column>
                  <div>부담스러웠던 상담신청</div>
                  <div>간편하게 신청해서 상담하세요.</div>
                </v-layout>
              </v-card-text>
              <v-btn outlined @click="free">무료상담</v-btn>
            </v-layout>
          </v-card-title>
        </v-card>
      </v-layout>
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
    free() {
      this.$router.push("/free");
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