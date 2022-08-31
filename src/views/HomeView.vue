<template>
  <div class="flex overflow-hidden">
    <div v-show="!change" class="w-0 md:w-72">
      <NavSidebar/>
    </div>
    <div v-show="change" class="hidden sm:block">
      <NavSideMin/>
    </div>
    <div class="w-full">
      <Content @nav="showNav"/>
    </div>
  </div>
</template>
<script>
import Content from '../components/Content'
import NavSidebar from "@/components/NavSidebar";
import NavSideMin from "@/components/NavSideMin";

export default {
  data(){
    return{
      change:false
    }
  },
  components:{
    NavSideMin,
    NavSidebar,
    Content
  },
  methods:{
    showNav(){
      this.change = !this.change
    }
  }
}
</script>
