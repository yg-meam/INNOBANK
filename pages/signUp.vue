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
        <v-btn text class="mr-8 blackText" @click="login">로그인</v-btn>
      </v-layout>
    </div>

    <v-layout align-center justify-center class="background">
      <v-card class="rounded-xl" flat height="500" width="300">
        <v-card-title style="height: 100%">
          <v-layout align-center justify-center column>
            <img src="/img/bulb.jpg" width="60" />
            <h2>INNOBANK</h2>
            <v-card-text>
              <v-layout align-center justify-center>
                <div>소중한 지식재산권을 지키는 방법!</div>
              </v-layout>
            </v-card-text>
            <v-text-field
              color="gray"
              v-model="email"
              dense
              label="이메일"
            ></v-text-field>
            <v-text-field
              color="gray"
              v-model="name"
              dense
              label="이름"
            ></v-text-field>
            <v-text-field
              color="gray"
              v-model="password"
              dense
              type="password"
              label="패스워드"
            ></v-text-field>
            <v-text-field
              color="gray"
              v-model="passwordCheck"
              dense
              type="password"
              label="패스워드 확인"
            ></v-text-field>
            <v-btn class="mt-3" rounded width="200" outlined @click="login"
              >회원가입</v-btn
            >
          </v-layout>
        </v-card-title>
      </v-card>
    </v-layout>
  </v-layout>
</template>

<script>
export default {
  data() {
    return {
      email: "",
      name: "",
      password: "",
      passwordCheck: "",
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
      if (!this.email) {
        return window.alert("이메일을 입력해주세요");
      } else if (!this.name) {
        return window.alert("이름을 입력해주세요");
      } else if (!this.password) {
        return window.alert("패스워드를 입력주세요");
      } else if (this.passwordCheck != this.password) {
        return window.alert("패스워드가 일치하지 않습니다");
      } else {
        return window.alert("가입되었습니다.");
      }
    },
    checkLogin() {},
  },
};
</script>

<style scoped>
.greyText {
  color: grey;
}
.blackText {
  color: black;
}
.phoneNumber {
  color: red;
}
.background {
  background-color: #eee;
}
.Innobank {
  font-weight: bold;
  font-size: 30px;
}
.loginCard {
  padding: 30%;
}
</style>
