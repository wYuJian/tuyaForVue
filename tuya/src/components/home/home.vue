<template>
    <div class="page">
        <el-row style="background:#000;">
            <el-col :span="16" :push='4'>
                <Header></Header>
            </el-col>
            <div style="width:100%">
                <el-col :span="16" :push='4'>
                    <div>
                        <el-carousel :interval="4000" type="card" width='100%'>
                            <el-carousel-item v-for="item in 6" :key="item">
                                <img :src="bannerSrc[item-1]" alt="">
                            </el-carousel-item>
                        </el-carousel>
                    </div>
                </el-col>
            </div>
        </el-row>
        <el-row>
            <el-col :span='16' :push="4">
                <div class="lsls-wrapper">
                    <Wrapper v-for='item in 3' :WrapperData='WrapperSrc[item-1]'></Wrapper>
                </div>
                <div class="wrapper">
                    <hello-title></hello-title>
                </div>
            </el-col>
        </el-row>
        <el-row style="background:#fff;border-top: 1px #eee solid;margin-top: 40px; border-bottom: 1px #eee solid;">
            <el-col :span="16" :push='4'>
                <Footer></Footer>
            </el-col>
        </el-row>
    </div>
</template>

<script type="text/ecmascript-6">
import Header from '@/components/header/header'
import Footer from '@/components/footer/footer'
import Wrapper from '@/components/home/wrapper/wrapper'
import HelloTitle from '@/components/home/helloTitle/helloTitle'
import Vue from 'vue'
import { Row, Col } from 'element-ui'
Vue.use(Row)
Vue.use(Col)
export default {
    name: 'Home',
    data() {
        return {
            bannerSrc: [
                'https://piccdn.gracg.com/uploadfile/photo/2018/5/pic_a4smesyxutgpwrjvn7toio2s3s7ycctc.jpg',
                'https://piccdn.gracg.com/uploadfile/photo/2018/5/pic_scqp7qjq6021jm6xzwf45snof1l1x4au.jpg',
                'https://piccdn.gracg.com/uploadfile/photo/2018/4/pic_44ejm2ysd8csbhglk5m2f8moijdrn376.jpg',
                'https://piccdn.gracg.com/uploadfile/photo/2018/6/pic_481mfouj4gqxpygkpe39em21nuu5hmf3.jpg',
                'https://piccdn.gracg.com/uploadfile/photo/2018/5/pic_gx10rtxffw558qsrlk4cg10lwkcj2gs3.jpg',
                'https://piccdn.gracg.com/uploadfile/photo/2018/4/pic_k6eax9rfpnvucxzcyhesc01zoc7q13i1.jpg'
            ],
            WrapperSrc: [
                {
                    txt: '少年三国志创三国计划同人绘画大赛-与梦相绘',
                    imgSrc:
                        'https://piccdn.gracg.com/uploadfile/photo/2018/4/pic_2k2mzutoq1pwp7djofumfepogfw0jlfx.jpg'
                },
                {
                    txt: '《魂斗罗》英雄归来像素风绘画大赛',
                    imgSrc:
                        'https://piccdn.gracg.com/uploadfile/photo/2018/5/pic_vjwu4qu6rf98gtrh1ibewo10idjcbew3.jpg'
                },
                {
                    txt: '剑网3九周年插画漫画大赛',
                    imgSrc:
                        'https://piccdn.gracg.com/uploadfile/photo/2018/5/pic_o5daxdhk77ki9e3epze8ojioq9f70vi1.jpg'
                }
            ]
        }
    },
    components: {
        Header,
        Footer,
        Wrapper,
        HelloTitle
    },
    mounted() {},
    methods: {}
}
</script>

<style scoped lang="less">
.el-carousel__item {
    img {
        width: 100%;
        height: 100%;
    }
}
.lsls-wrapper {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    margin-top: 40px;
}
</style>
