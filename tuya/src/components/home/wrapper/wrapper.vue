<script type="text/ecmascript-6">
export default {
    name: '',
    props: ['WrapperData'],
    data() {
        return {}
    },
    render() {
        return (
            <div class="wrapper">
                <a href="">
                    <img src={this.WrapperData.imgSrc} />
                </a>
                <p>{this.WrapperData.txt}</p>
            </div>
        )
    },
    components: {},
    mounted() {},
    methods: {}
}
</script>

<style scoped lang="less">
@import url(./wrapper.less);
</style>
