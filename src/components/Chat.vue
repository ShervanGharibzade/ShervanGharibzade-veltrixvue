<template>
    <div class="rounded w-[99%] overflow-hidden xl:w-1/3 bg-white m-2 p-4 border-b-2 border-gary-300">
      <h2 class="text-black pb-4">Chat</h2>
      <div class="overflow-hidden overflow-y-scroll h-72 border-gray-300">
        <div class="text-black">
          <div class="relative block text-right my-4">
            <span class="text-xs absolute -top-3.5 right-4 font-bold text-blue-500">Smith</span>
            <span class="bg-gray-300 rounded p-2 pt-4 mr-3">hi there</span>
            <span class="text-sm block text-gray-500 pt-2 mr-3">PM 14:25</span>
          </div>
          <div class="relative block my-4">
            <span class="bg-blue-200 rounded pt-4 p-2">
              hi
              <span class="text-xs relative -top-5 -left-4 font-bold text-blue-500">John Deo</span>
            </span>
            <span class="text-sm block text-gray-500 pt-2">PM 14:25</span>
          </div>
          <div class="relative block text-right my-4">
            <span class="text-xs absolute -top-3.5 right-4 font-bold text-blue-500">Smith</span>
            <span class="bg-gray-300 rounded pt-4 p-2 mr-3">how are u?</span>
            <span class="text-sm block text-gray-500 pt-2 mr-3">PM 14:25</span>
          </div>
          <div class="relative block my-4">
            <span class="bg-blue-200 rounded pt-4 p-2">
              fine bro
              <span class="text-xs absolute -top-3.5 left-1.5 font-bold text-blue-500">John Deo</span>
            </span>
            <span class="text-sm block text-gray-500 pt-2">PM 14:25</span>
          </div>
          <div class="relative block my-4">
            <span class="bg-blue-200 pt-4 rounded p-2">
              what about you?
              <span class="text-xs absolute -top-3.5 left-1.5 font-bold text-blue-500">John Deo</span>
            </span>
            <span class="text-sm block text-gray-500 pt-2 ">PM 14:25</span>
          </div>
          <div class="relative block text-right mt-8">

            <span class="bg-gray-300 pt-4 rounded p-2 mr-3">
              nothing bro
              <span class="text-xs absolute -top-3.5 right-4 font-bold text-blue-500">Smith</span>
            </span>
            <span class="text-sm block text-gray-500 pt-2 mr-3">PM 14:25</span>
          </div>
          <div v-for="msg in messages" class="relative block text-right my-8">

            <span class="bg-gray-300 rounded pt-4 p-2 pr-2 mr-3">
              {{msg}}
              <span class="text-xs relative -top-5 left-0 font-bold text-blue-500">Smith</span>
            </span>
            <span class="text-sm block text-gray-500 pt-2 mr-3">PM 14:25</span>
          </div>
        </div>
      </div>
      <div class="flex border-t-2 border-gary-800">
        <div class="flex-1 px-2">
          <input type="text" @keyup.enter="sendMessage" v-model="message" placeholder="Enter your message"
                 class="w-full border-2  bg-slate-50 rounded h-9 mt-2.5 pl-2 text-sm text-black ">
        </div>
        <button @click="sendMessage" class=" hover:bg-green-700 bg-green-600 p-1.5 text-white rounded my-2">Send</button>
      </div>
    </div>
  </template>

  <script>
    export default {
      data() {
        return {
          message: '',
          messages: [],
          sendIcon: ''
        }
      },
      methods: {
        sendMessage() {
          this.messages.push(this.message)
          this.message = '';
        },
        showProfile(){
          this.$emit('showProfile')
        }
      }
    }
  </script>
