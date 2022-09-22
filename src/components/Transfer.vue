<template>
 <div class="flex items-center justify-center bg-blue-proc py-8 lg:px-20 px-3 ">

      <div class="grid lg:grid-cols-2 lg:grid-flow-row py-8 lg:pl-20 space-y-4 space-x-6">
      <div class="rounded-lg bg-blue-gri ">
       <h4 class="text-white text-lg p-8">参与转账</h4>
       <p class="text-white text-base px-8  ">参与抽奖并赢得奖金</p>
       <h4 class="text-white text-base pl-8 py-5">抽奖流程如下：</h4>
       <p class="text-white text-base p-8 ">
      (1)转账低于最小金额时，不可以参与且不会退回，转账高于最大金额时，扣除手续费后退回 </p>
       <p class="text-white text-base py-4 px-8 ">
      (2) 仅支持整数币参与抽奖，小数部分自动忽略 </p>
      </div>
      <div class="rounded-lg bg-blue-gri py-10 px-16  ">
      <div class="py-24  rounded-lg bg-blue-imbd border-indigo-300  ">
      <img class="lg:pl-52 py-4 px-20" src="@/images/mark.svg" alt="mark">
      <p class="text-white lg:text-base text-sm text-center">向本平台指定钱包地址</p>
      <p class="text-white lg:text-base text-sm text-center">按规定金额转账后即成功参与抽奖</p>

       
      </div>
      </div>
      </div>
      

      </div>

</template>

<script>
 export default {
     name: 'Transfer',
 }
</script>