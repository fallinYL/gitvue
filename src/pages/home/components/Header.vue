 <template>
    <div class='header'>
        <div class="header-left">
            <div class='iconfont back-icon'>&#xe603;</div>
        </div>
        <div class="header-input">
            <span class='iconfont'>&#xe62c;</span>
          输入城市/景点/游玩主题
        </div>
        <div class="header-right">
            城市
            <span class='iconfont arrow-icon'>&#xe65a;</span>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang='stylus' scoped>
    @import '~styles/varibles.styl'
    .header
        display :flex
        height :0.86rem
        background : $bgColor
        color :white
        .header-left
            width :0.64rem
            float :left
            .back-icon
                padding-top:0.24rem
                text-align :center
                font-size:0.4rem
        .header-input
            flex :1
            height :0.64rem
            line-height:0.64rem
            margin-left:0.2rem
            margin-top:0.12rem
            padding-left:0.2rem
            background:white
            border-radius:0.1rem
            color:#ccc
        .header-right
            width :1.24rem
            float :right
            text-align :center
            padding-top:0.24rem
            .arrow-icon
                font-size :0.15rem
</style>
