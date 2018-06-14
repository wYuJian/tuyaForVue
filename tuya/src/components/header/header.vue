<script type="text/ecmascript-6">
import Vue from 'vue'
import { Row, Col } from 'element-ui'
Vue.use(Row)
Vue.use(Col)
export default {
    name: 'Header',
    data() {
        return {
          isMore:false,
          isMoreIndex:0
        }
    },
    render() {
        return (
            <div class="header">
                <div class="header-right">
                    <a href="" class="logo">
                        <img src="https://www.gracg.com/static/index/img/logo4.png" />
                    </a>
                    <div>
                        <ul class="menu-list">
                            <li class='poocgTopbar-info-menu' onMouseover={this.menuNavbarOver.bind(this,1)} onMouseout={this.menuNavbarOver.bind(this,1)}>
                                <a href="">作品</a>
                                {this.isMore &&this.isMoreIndex==1 ? <div class="poocgTopbar-info-menu__navbar">
                                  <a href="https://www.gracg.com/works/index/type/new" class="poocgTopbar-info-menu__navbar-item">最新发布</a>
                                  <a href="https://www.gracg.com/works/index/type/love" class="poocgTopbar-info-menu__navbar-item">最新获赞</a>
                                  <a href="https://www.gracg.com/works/index/type/hot" class="poocgTopbar-info-menu__navbar-item">热门作品</a>
                                  <a href="https://www.gracg.com/works/index/type/essence" class="poocgTopbar-info-menu__navbar-item">作品精选</a>
                                </div>:''}
                            </li>
                            <li>
                                <a href="">作者</a>
                            </li>
                            <li>
                                <a href="">活动</a>
                            </li>
                            <li>
                                <a href="">工作</a>
                            </li>
                            <li>
                                <a href="">客户端</a>
                            </li>
                            <li class='poocgTopbar-info-menu' onMouseover={this.menuNavbarOver.bind(this,2)} onMouseout={this.menuNavbarOver.bind(this,2)}>
                                <a href="">更多</a>
                                {this.isMore&&this.isMoreIndex==2 ? <div class="poocgTopbar-info-menu__navbar">
                                  <a href="https://www.gracg.com/about" class="poocgTopbar-info-menu__navbar-item">合作联系</a>
                                  <a href="https://www.gracg.com/about/help" class="poocgTopbar-info-menu__navbar-item">帮助中心</a>
                                  <a href="http://weibo.com/poocg?topnav=1&amp;wvr=6&amp;topsug=1" target="_blank" class="poocgTopbar-info-menu__navbar-item">官方微博</a>
                                </div>:''}
                                
                            </li>
                            <li>
                                <a href="">
                                    <i class="el-icon-search" />
                                </a>
                            </li>
                            <li>
                                <a href="" class="xueyuan">
                                    插画课程直播
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div>
                    <a>注册</a>
                    <a>登录</a>
                </div>
            </div>
        )
    },
    components: {},
    mounted() {},
    methods: {
      menuNavbarOver:function(index){
          this.isMoreIndex = index
          this.isMore = !this.isMore;
      }
    }
}
</script>

<style scoped lang="less">
@import url(./header.less);
</style>
