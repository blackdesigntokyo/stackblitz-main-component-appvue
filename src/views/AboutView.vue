<template>
  <!-- コンポーネントの表示部分を定義するVue.jsのテンプレートセクション -->
  <div class="about">
    <!-- ページのメインタイトルを表示するh1要素 -->
    <h1>This is an about page</h1>
    <!-- クリックイベントでonclick関数を呼び出すボタン要素 -->
    <!-- v-on:clickはVue.jsのイベントハンドリング用ディレクティブ -->
    <button v-on:click="onclick">トップへ</button>
  </div>
</template>

<script>
/* Vue.jsコンポーネントの動作を定義するJavaScript部分 */
export default {
  /* コンポーネントで使用するメソッド（関数）を定義するオブジェクト */
  methods: {
    /* ボタンクリック時に実行される関数 */
    onclick() {
      /* Vue Routerを使用してルートパス（'/'）へナビゲーションを実行 */
      /* this.$routerはVue Routerのインスタンスを指す */
      /* push()メソッドでプログラム的にページ遷移を行う */
      this.$router.push('/')
    }
  }
}
</script>