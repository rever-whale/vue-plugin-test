<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <simple-alert
      title="경고"
      msg="버전별 하위 비호환성 경고 - 예제로 배우는 PyQtopentutorials.org › module
2017. 12. 12. - 예제로 배우는 PyQt. 예제 중심으로 배우는 PyQt 프로그래밍. 예제로 배우는 PyQt 예제 중심으로 배우는 PyQt 프로그래밍. Opentutorials.org.
Xamarin.Forms - 단 하나의 버튼과 액션으로 구성된 경고 예제 ...riptutorial.com › xamarin-forms › example › 경고-표시
var alertResult = await DisplayAlert(
경고를 작성하는 방법? -경고문 작성 예제www.nasilyazilir.org › uyarilis-nasil-yazilir
경고 쓰는 방법? Tdk 철자법 가이드에 따르면 경고의 철자는 무엇입니까? 경고를 별도로 또는 인접하게 작성해야합니까?"
    />
    <Test />
  </div>
</template>

<script>
import { SimpleAlert, Test } from "./components";

export default {
  name: "App",
  components: {
    SimpleAlert,
    Test,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
