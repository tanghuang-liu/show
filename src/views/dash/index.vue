<template>
    <div class="pri">
          <Nav/>
          <div class="greet"></div>
          <div class="mybody">
               <el-row :gutter="30">
              <el-col :span="15">
                  <el-row><panel-group/></el-row>
                   <el-row>
                  <el-card class="map-card" shadow="never"></el-card>
                 </el-row>
              </el-col>
              <el-col :span="9">
                 <el-row>
                  <el-card class="box-card" shadow="never"></el-card>
                 </el-row>
                  <el-row> <el-card class="board-card" shadow="never"></el-card></el-row>
              </el-col>
            </el-row>
          </div>
         
    </div>
</template>
<script>
import Nav from './components/nav'
import PanelGroup from './components/PanelGroup'
export default {
    components:{
        Nav,
        PanelGroup
    }
}
</script>
<style lang="scss" scoped>
.pri{
    width: 100%;
    height: 2000px;
    background: #f2f2f2;
   .greet{
       margin-top: 50px;
       height: 70px;
       width: 100%;
   }
   .mybody{
       padding:0 30px 0 30px;
        .map-card{
         width: 100%;
         height: 643px;
       }
       .box-card{
         margin-top: 20px;
         width: 100%;
         height: 450px;
       }
       .board-card{
         margin-top: 20px;
         width: 100%;
         height: 300px;
       }
       
   }
}
::v-deep.el-card{
    border: none;
}
</style>