<template>
  <div id="app">
  <header class="d-flex flex-column flex-md-row align-items-center p-3 px-md-4 mb-3 bg-body border-bottom shadow-sm">
    <p class="h3 my-0 me-md-auto fw-normal">OLE Restaurant</p>
    <a class="btn btn-outline-primary" >รายการอาหาร {{product1.amount+product2.amount+product3.amount+product4.amount+product5.amount+product6.amount+product7.amount+product8.amount+product9.amount}} จาน </a>
  </header>
  <main class="container">
    <div class="pricing-header px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
    <div class="row row-cols-1 row-cols-md-3 mb-3 text-center">
    <div class="col">
      <div class="card mb-4 shadow-sm">
      <div class="card-header">
        <h4 class="my-0 fw-normal">{{product1.name}}</h4>
      </div>
      <div class="card-body">
        <img src="http://www.freakwhey.com/post_files/webboard/IMG1352897513.jpg"
        img height="150">
        <ul class="list-unstyled text-small">10 บาท</ul>
        <div id="example-1">
          <button type="button" class="w-100 btn btn-lg btn btn-outline-success" v-on:click= "product1.amount += 1" >เพิ่มรายการ</button>
          <br/><br/>
          <button type="button" class="w-100 btn btn-lg btn btn-outline-danger" v-on:click= "product1.amount -= 1" >ลดรายการ</button>
          <p>จำนวน {{ product1.amount }} รายการ </p>
        </div>
      </div>
    </div>
    </div>
    <div class="col">
      <div class="card mb-4 shadow-sm">
      <div class="card-header">
        <h4 class="my-0 fw-normal">{{product2.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRG1ayVfT9BhnxkhI402HXCGQTRzhwjs0LsZg&usqp=CAU"
        img height="150">
        <ul class="list-unstyled text-small">10 บาท</ul>
        <div id="example-2">
        <button type="button" class="w-100 btn btn-lg btn btn-outline-success" v-on:click= "product2.amount += 1" >เพิ่มรายการ</button>
        <br/><br/>
        <button type="button" class="w-100 btn btn-lg btn btn-outline-danger" v-on:click= "product2.amount -= 1" >ลดรายการ</button>
          <p>จำนวน {{ product2.amount }} รายการ </p>
        </div>
      </div>
    </div>
    </div>
    <div class="col">
      <div class="card mb-4 shadow-sm">
      <div class="card-header">
        <h4 class="my-0 fw-normal">{{product3.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://www.scholarship.in.th/wp-content/uploads/2015/06/32.jpg"
         img height="150">
        <ul class="list-unstyled text-small">50 บาท</ul>
        <div id="example-3">
          <button type="button" class="w-100 btn btn-lg btn btn-outline-success" v-on:click= "product3.amount += 1" >เพิ่มรายการ</button>
          <br/><br/>
          <button type="button" class="w-100 btn btn-lg btn btn-outline-danger" v-on:click= "product3.amount -= 1" >ลดรายการ</button>
          <p>จำนวน {{ product3.amount }} รายการ </p>
        </div>
      </div>
    </div>
    </div>
  </div>
    <div class="row row-cols-1 row-cols-md-3 mb-3 text-center">
    <div class="col">
      <div class="card mb-4 shadow-sm">
      <div class="card-header">
        <h4 class="my-0 fw-normal">{{product4.name}}</h4>
      </div>
      <div class="card-body">
        <img src="http://i2.wp.com/www.thaismescenter.com/wp-content/uploads/2018/10/e71.jpg?resize=660%2C339"
        img height="150">
        <ul class="list-unstyled text-small">45 บาท</ul>
        <div id="example-4">
          <button type="button" class="w-100 btn btn-lg btn btn-outline-success" v-on:click= "product4.amount += 1" >เพิ่มรายการ</button>
          <br/><br/>
          <button type="button" class="w-100 btn btn-lg btn btn-outline-danger" v-on:click= "product4.amount -= 1" >ลดรายการ</button>
          <p>จำนวน {{ product4.amount }} รายการ </p>
        </div>
      </div>
    </div>
    </div>
    <div class="col">
      <div class="card mb-4 shadow-sm">
      <div class="card-header">
        <h4 class="my-0 fw-normal">{{product5.name}}</h4>
      </div>
      <div class="card-body">
        <img src="http://i2.wp.com/www.thaismescenter.com/wp-content/uploads/2018/10/e81.jpg?resize=660%2C455"
        img height="150">
        <ul class="list-unstyled text-small">80 บาท</ul>
        <div id="example-5">
          <button type="button" class="w-100 btn btn-lg btn btn-outline-success" v-on:click= "product5.amount += 1" >เพิ่มรายการ</button>
          <br/><br/>
          <button type="button" class="w-100 btn btn-lg btn btn-outline-danger" v-on:click= "product5.amount -= 1" >ลดรายการ</button>
          <p>จำนวน {{ product5.amount }} รายการ </p>
        </div>
      </div>
    </div>
    </div>
    <div class="col">
      <div class="card mb-4 shadow-sm">
      <div class="card-header">
        <h4 class="my-0 fw-normal">{{product6.name}}</h4>
      </div>
      <div class="card-body">
        <img src="http://i0.wp.com/www.thaismescenter.com/wp-content/uploads/2018/10/e101.jpg?resize=660%2C441"
         img height="150">
        <ul class="list-unstyled text-small">55 บาท</ul>
        <div id="example-6">
          <button type="button" class="w-100 btn btn-lg btn btn-outline-success" v-on:click= "product6.amount += 1" >เพิ่มรายการ</button>
          <br/><br/>
          <button type="button" class="w-100 btn btn-lg btn btn-outline-danger" v-on:click= "product6.amount -= 1" >ลดรายการ</button>
          <p>จำนวน {{ product6.amount }} รายการ </p>
        </div>
      </div>
    </div>
    </div>
    <div class="col">
      <div class="card mb-4 shadow-sm">
      <div class="card-header">
        <h4 class="my-0 fw-normal">{{product7.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://lh3.googleusercontent.com/proxy/R1LYCSjZq4njfd7qksick9tu5tr9kQv5kFxBsvkX_k13J_SivvGJ8DmPhDjoPOjfawutX1qw5aVIPb3CixeQ2PA-2VfeG2ZikC1nc0yEg3P9pSC59Wqopoi6pMunp6Y"
         img height="150">
        <ul class="list-unstyled text-small">40 บาท</ul>
        <div id="example-6">
          <button type="button" class="w-100 btn btn-lg btn btn-outline-success" v-on:click= "product7.amount += 1" >เพิ่มรายการ</button>
          <br/><br/>
          <button type="button" class="w-100 btn btn-lg btn btn-outline-danger" v-on:click= "product7.amount -= 1" >ลดรายการ</button>
          <p>จำนวน {{ product7.amount }} รายการ </p>
        </div>
      </div>
    </div>
    </div>

<div class="col">
      <div class="card mb-4 shadow-sm">
      <div class="card-header">
        <h4 class="my-0 fw-normal">{{product8.name}}</h4>
      </div>
      <div class="card-body">
        <img src="https://magazine.foodpanda.co.th/wp-content/uploads/sites/14/2019/11/%E0%B9%81%E0%B8%81%E0%B8%87%E0%B8%88%E0%B8%B7%E0%B8%94.jpg"
         img height="150">
        <ul class="list-unstyled text-small">40 บาท</ul>
        <div id="example-6">
          <button type="button" class="w-100 btn btn-lg btn btn-outline-success" v-on:click= "product8.amount += 1" >เพิ่มรายการ</button>
          <br/><br/>
          <button type="button" class="w-100 btn btn-lg btn btn-outline-danger" v-on:click= "product8.amount -= 1" >ลดรายการ</button>
          <p>จำนวน {{ product8.amount }} รายการ </p>
        </div>
      </div>
    </div>
    </div>

    <div class="col">
      <div class="card mb-4 shadow-sm">
      <div class="card-header">
        <h4 class="my-0 fw-normal">{{product9.name}}</h4>
      </div>
      <div class="card-body">
        <img src="http://i0.wp.com/www.thaismescenter.com/wp-content/uploads/2018/10/e121.jpg?resize=660%2C399"
         img height="150">
        <ul class="list-unstyled text-small">45 บาท</ul>
        <div id="example-6">
          <button type="button" class="w-100 btn btn-lg btn btn-outline-success" v-on:click= "product9.amount += 1" >เพิ่มรายการ</button>
          <br/><br/>
          <button type="button" class="w-100 btn btn-lg btn btn-outline-danger" v-on:click= "product9.amount -= 1" >ลดรายการ</button>
          <p>จำนวน {{ product9.amount }} รายการ </p>
        </div>
      </div>
    </div>
    </div>
    
    
      
  </div>
  <p class="h4 my-0 me-md-auto fw-normal">รายการอาหารที่เลือก</p>
  <header class="d-flex flex-column flex-md-row align-items-mide p-3 px-md-4 mb-3 bg-body border-bottom shadow-sm">
  <div v-if="product1.amount >= 1">
    ข้าวสวย
    <img src="http://www.freakwhey.com/post_files/webboard/IMG1352897513.jpg" width="60"  height=“60”>
    <p1> x{{ product1.amount }} </p1>
  </div>
  <div v-if="product2.amount >= 1">
    ข้าวเหนียว
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRG1ayVfT9BhnxkhI402HXCGQTRzhwjs0LsZg&usqp=CAU" width="60"  height=“60”>
    <p1> x{{ product2.amount }}</p1>
  </div>
  <div v-if="product3.amount >= 1">
    ต้มยำกุ้ง
    <img src="https://www.scholarship.in.th/wp-content/uploads/2015/06/32.jpg" width="60"  height=“60”>
    <p1> x{{ product3.amount }}</p1>
  </div>
  <div v-if="product4.amount >= 1">
    ผัดผักรวมมมิตร
    <img src="http://i2.wp.com/www.thaismescenter.com/wp-content/uploads/2018/10/e71.jpg?resize=660%2C339" width="60"  height=“60”>
    <p1> x{{ product4.amount }}</p1>
  </div>
  <div v-if="product5.amount >= 1">
    กุ้งผัดพริกเผา
    <img src="http://i2.wp.com/www.thaismescenter.com/wp-content/uploads/2018/10/e81.jpg?resize=660%2C455" width="60"  height=“60”>
    <p1> x{{ product5.amount }}</p1>
  </div>
  <div v-if="product6.amount >= 1">
    ผัดคะน้าปลาเค็ม
    <img src="http://i0.wp.com/www.thaismescenter.com/wp-content/uploads/2018/10/e101.jpg?resize=660%2C441" width="60"  height=“60”>
    <p1> x{{ product6.amount }}</p1>
  </div>
  <div v-if="product7.amount >= 1">
    หมูผัดพริกหยวก
    <img src="https://lh3.googleusercontent.com/proxy/R1LYCSjZq4njfd7qksick9tu5tr9kQv5kFxBsvkX_k13J_SivvGJ8DmPhDjoPOjfawutX1qw5aVIPb3CixeQ2PA-2VfeG2ZikC1nc0yEg3P9pSC59Wqopoi6pMunp6Y" width="60"  height=“60”>
    <p1> x{{ product7.amount }}</p1>
  </div>
  <div v-if="product8.amount >= 1">
    ต้มจืดเต้าหู้หมูสับ
    <img src="https://magazine.foodpanda.co.th/wp-content/uploads/sites/14/2019/11/%E0%B9%81%E0%B8%81%E0%B8%87%E0%B8%88%E0%B8%B7%E0%B8%94.jpg" width="60"  height=“60”>
    <p1> x{{ product8.amount }}</p1>
  </div>
  <div v-if="product9.amount >= 1">
    ผัดผักบุ้ง
    <img src="http://i0.wp.com/www.thaismescenter.com/wp-content/uploads/2018/10/e121.jpg?resize=660%2C399" width="60"  height=“60”>
    <p1> x{{ product9.amount }}</p1>
  </div>
  </header>
  <h4>ราคารวม {{ sum+product1.amount*product1.price+product2.amount*product2.price+product3.amount*product3.price+product4.amount*product4.price+product5.amount*product5.price+product6.amount*product6.price+product7.amount*product7.price+product8.amount*product8.price+product9.amount*product9.price }} บาท</h4>
  <button type="button" class="w-50 btn btn-lg btn-outline-primary" v-on:click="say('รับรายการอาหารสำเร็จ')" >สั่งอาหาร</button>
  <br>
  <br>
  <input  class="btn btn-dark" type="button" value="Reset" onClick="javascript:location.reload();">
  </div>
  </main>
  </div>
</template> 

<script>
export default {
  name: 'App',
  data(){
    return{
      product1:{
        name:"ข้าวสวย",
        price:10,
        amount:0
      },
      product2:{
        name:"ข้าวเหนียว",
        price:10,
        amount:0
      },
      product3:{
        name:"ต้มยำกุ้ง",
        price:50,
        amount:0
      },
      product4:{
        name:"ผัดผักรวมมมิตร",
        price:45,
        amount:0
      },
      product5:{
        name:"กุ้งผัดพริกเผา",
        price:80,
        amount:0
      },
      product6:{
        name:"ผัดคะน้าปลาเค็ม",
        price:55,
        amount:0
      },
      product7:{
        name:"หมูผัดพริกหยวก",
        price:40,
        amount:0
      },
      product8:{
        name:"ต้มจืดเต้าหู้หมูสับ",
        price:40,
        amount:0
      },
      product9:{
        name:"ผัดผักบุ้ง",
        price:45,
        amount:0
      },
      
      
      sum: 0,count:0,say: function (message) {
      alert(message)
    }
    }
  }
}
</script>