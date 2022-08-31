<template>
  <div class="bg-zine-100 h-full relative overflow-hidden">
    <NavTop @nav="e" @setting="CloseSetting"/>
    <div class="transition-transform duration-300">
      <SettingBar @close="CloseSetting" v-show="show"/>
    </div>
    <div class="px-4 mt-14 md:mt-0 bg-zinc-100 text-zinc-500">
      <div class="flex py-5 px-2">
        <p class="flex-1 text-sm">
          <span class="font-bold text-lg"> Dashboard </span>
          <br>
          Welcome to Veltrix Dashboard
        </p>
        <button class="bg-blue-600 hidden md:block text-white px-4 my-1 transition duration-200 hover:bg-blue-700 rounded cursor-pointer">setting</button>
      </div>
      <div class="grid xl:grid-cols-4 lg:grid-cols-2 md:grid-cols-2 grid-cols-1">
        <Card
            price="1,685"
            num="+12%"
            icon="fa fa-object-group"
            title="orders"
            color="bg-green-500"
        />
        <Card
            price="52,368"
            num="-28%"
            icon="fa fa-clipboard"
            title="revenue"
            color="bg-red-500"
        />
        <Card
            price="15,8"
            num="00%"
            icon="fa fa-pencil"
            title="average price"
            color="bg-blue-500"
        />
        <Card
            price="2436"
            num="+84%"
            icon="fa fa-briefcase"
            title="product sold"
            color="bg-yellow-500"
        />
      </div>
    </div>
    <div class="grid w-[97%] my-2 mx-3 lg:flex rounded overflow-hidden">
      <ChartMax/>
      <ChartMin class="mt-5 md:mt-0"/>
    </div>
    <div class="xl:flex grid">
      <ProgressCirle class="w-full"/>
      <Activity class="w-full mt-2"/>
      <Clinet class="w-full"/>
    </div>
    <div class="xl:flex grid">
      <Latest class="w-full"/>
      <Chat class="w-full"/>
    </div>
  </div>
</template>
<script>
import NavTop from "@/components/NavTop";
import Card from "@/components/Card";
import ProgressCirle from "@/components/ProgressCircle";
import Activity from "@/components/Activity";
import Clinet from "@/components/Clinet";
import Latest from "@/components/Latest";
import Chat from "@/components/Chat";
import SettingBar from "@/components/SettingBar";
import ChartMax from "@/components/ChartMax";
import ChartMin from "@/components/ChartMin";

export default {
  components: {ChartMin, ChartMax, Chat, Latest, Clinet, Activity, ProgressCirle, Card, NavTop , SettingBar},
  methods:{
  CloseSetting(){
    this.show = !this.show
  },
    e(){
    this.$emit('nav')
    }
  },
  data(){
    return{
      show:false
    }
  }
}
</script>
