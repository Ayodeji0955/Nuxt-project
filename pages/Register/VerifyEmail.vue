<template>
  <div class="login">
    <div class="row align-items-center">
      <div class="col-md-6 login__main-col">
        <div class="container py-4">
          <div class="formbg-outer">
            <div class="formbg">
              <div class="formbg-inner padding-horizontal--48">
                <div class=" text-center py-4">
                  <img src="~@/assets/images/img_1/favicon.png">
                </div>
                <h1 class="padding-bottom--12 text-center">
                  Confirm Email
                </h1>
                <span class="padding-bottom--15 text-center">Information link has been sent to your email address email address</span>
                <div class=" text-center py-5 mail">
                  <img src="~@/assets/images/img_1/mail.png">
                </div>
                <form id="stripe-login">
                  <a class="ssolink" href="#">Forgot password? </a>
                  <div class="field padding-bottom--24 py-3 px-4">
                    <input type="submit" name="submit" value="Sign in">
                  </div>
                </form>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6 login__sub-col" />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage'

})

</script>

<style lang="scss">
.login {
  &__sub-col {
    background-image: url('~@/assets/images/img_1/wrk.png');
    background-position:center;
    background-size:cover;
    // padding-top: 7rem;
    height: 100vh;
  }
}
* {
    padding: 0;
    margin: 0;
    color: #1a1f36;
    box-sizing: border-box;
    word-wrap: break-word;
    font-family: -apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Ubuntu,sans-serif;
}
.mail img {
  width: 65px;
  height: 65px;
  text-align: center;
}
body {
    min-height: 100%;
    background-color: #ffffff;
    margin: 0;
}
h1 {
    letter-spacing: -1px;
}
a {
  color: #5A27D5;
  text-decoration: unset;
}
.login-root {
    background: #fff;
    display: flex;
    width: 100%;
    min-height: 100vh;
    overflow: hidden;
}
.loginbackground {
    min-height: 692px;
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    top: 0;
    z-index: 0;
    overflow: hidden;
}
.flex-flex {
    display: flex;
}
.align-center {
  align-items: center;
}
.center-center {
  align-items: center;
  justify-content: center;
}
.box-root {
    box-sizing: border-box;
}
.flex-direction--column {
    -ms-flex-direction: column;
    flex-direction: column;
}
.loginbackground-gridContainer {
    display: -ms-grid;
    display: grid;
    -ms-grid-columns: [start] 1fr [left-gutter] (86.6px) [left-gutter] 1fr [end];
    grid-template-columns: [start] 1fr [left-gutter] repeat(16,86.6px) [left-gutter] 1fr [end];
    -ms-grid-rows: [top] 1fr [top-gutter] (64px) [bottom-gutter] 1fr [bottom];
    grid-template-rows: [top] 1fr [top-gutter] repeat(8,64px) [bottom-gutter] 1fr [bottom];
    justify-content: center;
    margin: 0 -2%;
    transform: rotate(-12deg) skew(-12deg);
}
.padding-top--64 {
  padding-top: 4rem;
}
.padding-top--24 {
  padding-top: 1.5rem;
}
.padding-top--48 {
  padding-top: 3rem;
}
.padding-bottom--24 {
  padding-bottom: 1.5rem
}
.padding-horizontal--48 {
  padding: 1.5rem;
}
.padding-bottom--15 {
  padding-bottom: 0.5rem;
  color: #404040;
  font-family: 'Inter';
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
}
.padding-bottom--12 {
  padding-bottom: 0.75rem;
  font-family: 'Inter';
  font-style: normal;
  font-weight: 600;
  font-size: 24px;
  line-height: 20px;
  color: #404040;
}
.formbg {
  margin: 0px auto;
  width: 100%;
  max-width: 448px;
  background: white;
  border-radius: 4px;
}
span {
  display: block;
  font-size: 20px;
  line-height: 28px;
  color: #1a1f36;
}
label {
  margin-bottom: 10px;
}
.reset-pass a,label {
  font-size: 14px;
  font-weight: 600;
  display: block;
}
.reset-pass > a {
  text-align: right;
  margin-bottom: 10px;
}
.grid--50-50 {
  display: grid;
  grid-template-columns: 50% 50%;
  align-items: center;
}
.field input {
  font-size: 16px;
  line-height: 28px;
  padding: 8px 16px;
  width: 100%;
  min-height: 44px;
  border: unset;
  border-radius: 4px;
  outline-color: rgb(84 105 212 / 0.5);
  background-color: linear-gradient(90.73deg, #5A27D5 0%, #5F27D3 32.36%, #AE2EC4 100%);
  box-shadow: rgba(0, 0, 0, 0) 0px 0px 0px 0px,
              rgba(0, 0, 0, 0) 0px 0px 0px 0px,
              rgba(0, 0, 0, 0) 0px 0px 0px 0px,
              rgba(60, 66, 87, 0.16) 0px 0px 0px 1px,
              rgba(0, 0, 0, 0) 0px 0px 0px 0px,
              rgba(0, 0, 0, 0) 0px 0px 0px 0px,
              rgba(0, 0, 0, 0) 0px 0px 0px 0px;
}

.input[type="submit"] {
  background: linear-gradient(90.73deg, #5A27D5 0%, #5F27D3 32.36%, #AE2EC4 100%);
  color: #fff;
  font-weight: 600;
      cursor: pointer;
}
.field-checkbox input {
  width: 20px;
  height: 15px;
  margin-right: 5px;
  box-shadow: unset;
  min-height: unset;
}
.field-checkbox label {
  display: flex;
  align-items: center;
  margin: 0;
}
a.ssolink {
  display: block;
  text-align: center;
  font-weight: 600;
}
.footer-link span {
  font-size: 14px;
  text-align: center;
}
.listing a {
  color: #697386;
  font-weight: 600;
  margin: 0 10px;
}
</style>
