<script type="text/ecmascript-6">
export default {
    name: '',
    data() {
        return {}
    },
    render() {
        return (
            <div class='TheHomeWorksList' onMouseover={this.mouseOver}>
                <div>
                    <a href="" class="imgbox">
                        <img src="https://piccdn.gracg.com/uploadfile/photo/2018/6/pic_2niq6zogm57s98yskaaoexuqqq1967n4.jpg!/scale/9/clip/298x298a25s0/format/jpg/rotate/auto" />
                        <div class='tool'>
                            <span class='new_workLvIcon_inlineB_jh'></span>
                            <span class='worknum'></span>
                        </div>
                    </a>
                    
                </div>
                <div class="infobox">
                    <p class='titles'>《逆光》</p>
                    <div class='info'>
                        <span class='icon-imgbg-hpw_see hpw_see'><i class='iconfont'>&#xe608;</i>81</span>
                        <span class='icon-imgbg-hpw_love hpw_love'><i class='iconfont'>&#xe64e;</i>2</span>
                        <span class='icon-imgbg-hpw_pl hpw_pl'><i class='iconfont'>&#xe60d;</i>1</span>
                    </div>
                    <div class='userinfo'>
                        <a href="">
                            <img class='faces' src="https://piccdn.gracg.com/uploadfile/user/2018/4/pic_ckh37nwlmsnunwrhia7r460v760fy9de.jpg!newface/both/50x50" />
                            一碗乌冬面
                        </a>
                    </div>
                    <div class="tags">
                        <a
                            href="https://www.gracg.com/tags/index/q/火影忍者"
                            target="_blank"
                            class="btn btn-light btn-sm"
                        >
                            火影忍者
                        </a>
                        <a
                            href="https://www.gracg.com/tags/index/q/火影忍者"
                            target="_blank"
                            class="btn btn-light btn-sm"
                        >
                            火影忍者
                        </a>
                    </div>
                </div>
            </div>
        )
    },
    components: {},
    mounted() {},
    methods: {
        mouseOver(){
            
        }
    }
}
</script>

<style scoped lang="less">
@import url(./TheHomeWorksList.less);
</style>
