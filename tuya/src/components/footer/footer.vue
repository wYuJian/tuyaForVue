<script type="text/ecmascript-6">
export default {
    name: 'Footer',
    data() {
        return {}
    },
    render(){
        return(
            <div class='footer'>
                <div>
                    <a href=''>首页</a>
                    <a href=''>关于</a>
                    <a href=''>合作联系</a>
                    <a href=''>客户端下载</a>
                    <span>友情链接:</span><a href=''>帮助中心</a>
                    <a href=''>CGToken.io</a>
                </div>
                <p>涂鸦王国（gracg.com）会员所发布展示的原创作品版权归原作者所有，任何商业用途均须联系作者。</p>
                <p>如未经授权用作他处，作者将保留追究侵权者法律责任的权利。 </p>
                <p>Copyright © 2003 - 2018   网站备案：闽ICP备16007928号-2 网络文化经营许可证：闽网文(2018)1334-071号</p>
            </div>
        )
    },
    components: {},
    mounted() {},
    methods: {}
}
</script>

<style scoped lang="less">
@import url(./footer.less);
</style>
