<template>
    <div id="indexContent">
        <el-row>
            <el-card>
                <el-carousel :interval="4000" type="card" height="330px">
                    <el-carousel-item v-for="item in imgList" :key="item">
                        <el-tooltip class="item" effect="dark" :content="item.title" placement="top">
                            <el-image :src="item.url" ></el-image>
                        </el-tooltip>
                    </el-carousel-item>
                </el-carousel>
            </el-card>
        </el-row>

        <el-row>
            <el-card>
                <el-row>
                    <el-col :span="5">
                        <el-image src="https://img20.360buyimg.com/pop/s1180x940_jfs/t1/191791/25/19504/72405/6120ecc6Eb4e24aca/e68080725601f1cc.jpg.webp"></el-image>
                    </el-col>
                    <el-col :span="1"><div class="none"></div></el-col>
                    <el-col :span="5">
                        <el-image src="https://img30.360buyimg.com/pop/s1180x940_jfs/t1/186613/4/19634/98444/612366dfEcd32df9d/7ea284b01d94dc3e.jpg.webp"></el-image>
                    </el-col>
                    <el-col :span="1"><div class="none"></div></el-col>
                    <el-col :span="5">
                        <el-row class="customCard">
                            <el-row >

                                <span class="channelItemName">创意礼品</span>
                                <span class="channelItemTitle">表达美好心意</span>
                            </el-row>
                            <el-row >
                                <el-col :span="2"><div class="none"></div></el-col>
                                <el-col :span="9">
                                    <el-image src="http://img13.360buyimg.com/pop/s1180x940_jfs/t1/190022/28/14456/53328/60fa9346E2d755a05/dd50f3cce807ae80.jpg.webp"></el-image>
                                </el-col>
                                <el-col :span="2"><div class="none"></div></el-col>
                                <el-col :span="9">
                                    <el-image src="https://imgcps.jd.com/ling4/10021292212114/5bel5ZOB6LStUExVU-S4k-S6qw/5ruhMeWFg-S6qzguNeaKmA/p-5bd8253082acdd181d02fa47/e1a07287/cr/s/q.jpg"></el-image>
                                </el-col>

                            </el-row>
                        </el-row>
                    </el-col>
                </el-row>
            </el-card>
        </el-row>
    </div>
</template>

<script>
    export default {
        name: "indexContent",
        components:{},
        data(){
            return{
                imgList:[
                    {title:"腾讯ROG游戏手机5s系列",url:"https://img.alicdn.com/tfs/TB1wOidVWL7gK0jSZFBXXXZZpXa-520-280.jpg"},
                    {title:"京选好物",url:"https://imgcps.jd.com/ling4/100021781178/5Lqs6YCJ5aW96LSn/5L2g5YC85b6X5oul5pyJ/p-5f3a47329785549f6bc7a6f1/c451bb0d/cr/s/q.jpg"},
                    {title:"范思哲石英表",url:"https://gtms02.alicdn.com/tps/i2/TB10vPXKpXXXXacXXXXvKyzTVXX-520-280.jpg"},
                    {title:"8月来电好物季",url:"https://gtms03.alicdn.com/tps/i3/TB1gXd1JXXXXXapXpXXvKyzTVXX-520-280.jpg"},
                    {title:"ThinkBook",url:"https://img.alicdn.com/tfs/TB1FjZ7VWL7gK0jSZFBXXXZZpXa-520-280.png"},
                    {title:"电竞博物志",url:"https://gtms01.alicdn.com/tps/i1/TB1r4h8JXXXXXXoXXXXvKyzTVXX-520-280.jpg"},

                ]
            }
        }
    }
</script>

<style scoped>
.channelItemName{
    margin-left:17px;
    font-size: 1.3em;
    font-weight: bolder;
}
.channelItemTitle{
    margin-left:10px;
    font-size: 0.7em;
    color:#909399;
}
.customCard{
    border:1px solid #DCDFE6;
    border-radius: 5px;
    padding:20px 0;
}
</style>