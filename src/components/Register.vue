<template>
 <div class="flex items-center justify-center bg-blue-proc py-8 lg:px-20 px-3 ">

      <div class="grid lg:grid-cols-2 lg:grid-flow-row py-8 lg:pl-20 space-y-4 space-x-6">
      <div class="rounded-lg bg-blue-gri ">
       <h4 class="text-white text-lg p-8">注册钱包</h4>
       <p class="text-white text-base p-8 ">去中心化钱包的数据都是区块链上的数据，而中心化钱包的数据则依赖钱包服务商自己的账本</p>
       <h4 class="text-white text-lg pl-8">举个例子</h4>
       <p class="text-white text-base p-8 ">
       我们在交易所的钱包就是中心化钱包，我们往交易所指定的地址转账，然后交易所在自己的账本上记录了我们的充值记录，此后每做一次充值转账，交易所直接在他的账本上进行记录，
       这整个过程完全没有发生在区块链上。
       因此我们需要注册一个属于自己的去中心化钱包 </p>
      </div>
      <div class="rounded-lg bg-blue-gri py-10  ">
      
      <div class="flex items-center justify-center rounded-lg">
      <div class=" grid grid-cols-3 grid-flow-row bg-white rounded-lg divide-y ">
      <div class="rounded-tl-lg bg-blue-yellow px-4"><p class="text-white text-2xl font-semibold p-6 ">平台</p></div>
      <div class="bg-blue-yellow px-4"><p class="text-white text-2xl font-semibold py-6 ">网址</p></div>
      <div class="rounded-tr-lg bg-blue-yellow px-4"><p class="text-white text-2xl font-semibold py-6">教程</p></div>
      <div class=""><img class="pt-4 text-center" src="@/images/1.svg" alt="first"></div>
      <div class=""><p class="text-center text-black text-base font-semibold p-6">token.im</p></div>
      <div class=""><p class="text-blue-brown text-base font-semibold p-6">查看教程</p></div>
      <div class=""><img class="pt-4" src="@/images/2.svg" alt="nd"></div>
      <div class=""><p class="text-center text-black text-base font-semibold p-6">trustwallet.com</p></div>
      <div class=""><p class="text-blue-brown text-base font-semibold p-6">查看教程</p></div>
      <div class=""><img class="pt-4" src="@/images/3.png" alt="rd"></div>
      <div class=""><p class="text-center text-black text-base font-semibold p-6">ownbit.io</p></div>
      <div class=""><p class="text-blue-brown text-base font-semibold p-6">查看教程</p></div>
      <div class=""><img class="pt-4" src="@/images/4.svg" alt="th"></div>
      <div class=""><p class="text-center text-black text-base font-semibold p-6">tronlink.org</p></div>
      <div class=""><p class="text-blue-brown text-base font-semibold p-6">查看教程</p></div>
      <div class=""><img class="pt-4" src="@/images/5.svg" alt="th"></div>
      <div class=""><p class="text-center text-black text-base font-semibold p-6">bitpie.com</p></div>
      <div class=""><p class="text-blue-brown text-base font-semibold p-6">查看教程</p></div>
      

      </div>
      </div>
      </div>
      </div>

      </div>

</template>

<script>
 export default {
     name: 'Register',
 }
</script>