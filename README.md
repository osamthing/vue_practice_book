# Vue.js for Green

## プロジェクトを作成する

vueを使うディレクトリの作成。ここではPROJECT_DIR
````
mkdir -m 755 PROJECT_DIR
cd PROJECT_DIR
````

node.jsのバージョンの確認
````
node -v
v9.2.0
````

vueをnpmでインストールする
````
npm install vue@csp
````
これで準備は完了です。

## ソースを書く
````
<!DOCTYPE html>
<html>

<head>
<script type="text/javascript" src="../node_modules/vue/dist/vue.min.js"></script>
</head>

<div id="app">
    <p>{{ message }}</p>
    <input v-model="message">
</div>

<script>
new Vue({
    el: '#app',
    data: {
        message: 'Hello Vue.js!'
    }
})
</script>

</html>
````
フォームに文字を入れたら動的に同じ描画をしてくれます。

--------------------------
[10分で始めるVue.js(基本編)](https://qiita.com/hikarut/items/a71f065feaa3f5bca5e3)
