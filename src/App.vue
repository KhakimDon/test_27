<script setup lang="ts">
import { onMounted, ref } from 'vue';
import Cursor from './components/Cursor.vue';
import './style.css'

const header = ref(false)
onMounted(() =>{
  window.onscroll = () => {
    if(window.pageYOffset > 200){
      header.value = true
    }else{
      header.value = false
    }
  }
})


</script>

<template>
  <div>
    <cursor/>
    <header :class="{activeheader: header}" class="header h-[80px] z-[999] fixed w-[100%] top-0 flex justify-between">
      <div class="flex items-center h-[100%] w-[max-content]">
        <div
          class="hoveritems overflow-hidden flex items-center bg-[black] h-[100%] cursor-pointer px-[30px] text-white gap-[10px] justify-center">
          <svg fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-8">
            <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 9h16.5m-16.5 6.75h16.5" />
          </svg>
          <span class="text-[18px] font-[Montserrat]">Menu</span>
        </div>
        <div class="hoveritem bg-white h-[100%] flex items-center justify-center pb-[5px] px-[20px]">
          <img class=" h-[28px] removeblock" src="https://klassen.eu/image/logos/klassen_black.svg" alt="logo">
          <img class=" h-[28px] hoverblock" src="https://klassen.eu/image/logos/klassen_black.svg" alt="logo">
        </div>
      </div>
      <div class="texts flex items-center">
        <div class="text-white font-[Montserrat] pr-[20px] flex flex-col items-end">
          <p>festnetz: <a class="font-[700] hover:underline" href="tel:+998915491754">+998 (91) 549-17-54</a></p>
          <p>mobil: <a class="font-[700] hover:underline" href="tel:+998915491754"> +998 (91) 549-17-54</a></p>
        </div>
        <div class="bg-white text-black searcher h-[100%] flex items-center justify-center px-[30px] cursor-pointer">
          <svg fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor" class="size-6">
            <path stroke-linecap="round" stroke-linejoin="round"
              d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z" />
          </svg>
        </div>
      </div>
    </header>
    <main >
      <section class="first z-[1] flex items-center justify-center relative h-[90vh] bg-[#2e2d2d]">
        <div class="text-white z-[44] max-w-[1100x] w-[1200px]">
          <span class="font-[Montserrat] font-[400] text-[18px]">Basierend auf</span>
          <h1 class="font-[mersb] font-[600] text-[48px]">Mercedes-Benz</h1>
          <p class="font-[Montserrat] font-[500] max-w-[500px] text-[18px]">Lorem, ipsum dolor sit amet consectetur
            adipisicing elit. Reprehenderit nobis reiciendis.</p>
          <button
            class="btn rounded-none mt-[40px] text-[16px] bg-[transparent] text-[white] hover:bg-[white] hover:text-[black] font-[Montserrat] px-[40px] h-[50px]">ALLE
            MODELLE</button>
        </div>
        <video class="w-[100%] z-[-2] h-[100%] top-0 object-cover object-center absolute" muted autoplay
          src="./assets/video.mp4"></video>
      </section>
      <section class="h-[50vh] bg-[white]">
        <div class="max-w-[1200px] gap-[100px] mx-auto flex justify-between items-center h-[100%]">
          <div class="flex flex-col gap-[20px] text-[32px]">
            <img class=" h-[55px]" src="https://klassen.eu/image/logos/klassen_black.svg" alt="logo">
            <span class="leading-[32px]">Automobile GmbH</span>
          </div>
          <div class="flex-1 font-[Montserrat] font-[500]">
            Wir freuen uns, Sie als Liebhaber exklusiver Automobile auf unserer Webseite begrüßen zu dürfen. Wir laden
            Sie
            ein, die KLASSEN - Welt zu erkunden. Erleben Sie bei einem Streifzug durch unsere über 20-jährige
            Firmengeschichte, wie wir die Fahrzeugveredelung bis heute revolutioniert und perfektioniert haben.
            <p class="font-[700] underline"> Besuchen Sie uns in Minden in unserem Showroom und überzeugen Sie sich
              selbst von unserer Arbeit und ihrer
              Qualität..</p>
          </div>
        </div>
      </section>
      <section class="h-[150vh]">
        <div class="max-w-[1440px] flex w-[100%] mx-auto">
          <div class="w-[50%]">
            <!-- <img src="" alt="image"> -->
             <div class="imgimg h-[33.3%]"></div>
             <div class="imgimg2 h-[33.3%] mt-[1px]"></div>
             <div class="imgimg3 h-[33.3%] mt-[1px]"></div>
          </div>
          <div class="w-[50%] p-[30px] font-[Montserrat]">
            <p>
              <span class="font-[mersb] text-[28px] mb-[10px] block">Mercedes-Benz.</span> 
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium rem recusandae sequi nam nesciunt
              earum maxime et sapiente a dicta facilis quae quam, ducimus incidunt quis magnam voluptatibus accusamus
              dolor odit iste quibusdam eligendi dolorem accusantium. Dignissimos qui fuga non, totam, nobis nisi
              aperiam veritatis blanditiis tempore et odit commodi magni laboriosam animi dicta. Rerum assumenda
              accusantium ab voluptas odit laudantium eveniet similique molestias sed, maxime quis ad numquam ratione.
              Ipsum repudiandae, optio debitis reiciendis iste dolores aperiam perspiciatis quibusdam, exercitationem
              sint doloremque velit culpa impedit repellendus, quia quod quisquam hic libero? Minus dolorum ullam
              tenetur ad enim illum explicabo tempora, assumenda temporibus consequuntur alias debitis magnam eum
              consequatur magni. Suscipit amet mollitia accusantium, quod asperiores eaque libero vel rerum, neque
              possimus laborum, dolor totam reprehenderit aspernatur. Aspernatur eius iste dicta, odio ipsam
              consectetur, tempore quis praesentium expedita sed aliquid!
            </p>
            <p class="mt-[120px]">
              <span class="font-[mersb] text-[28px] mb-[10px] block">Other Mercedes-Benz.</span> <br>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium rem recusandae sequi nam nesciunt
              earum maxime et sapiente a dicta facilis quae quam, ducimus incidunt quis magnam voluptatibus accusamus
              dolor odit iste quibusdam eligendi dolorem accusantium. Dignissimos qui fuga non, totam, nobis nisi
              aperiam veritatis blanditiis tempore et odit commodi magni laboriosam animi dicta. Rerum assumenda
              accusantium ab voluptas odit laudantium eveniet similique molestias sed, maxime quis ad numquam ratione.
              Ipsum repudiandae, optio debitis reiciendis iste dolores aperiam perspiciatis quibusdam, exercitationem
              sint doloremque velit culpa impedit repellendus, quia quod quisquam hic libero? Minus dolorum ullam
              tenetur ad enim illum explicabo tempora, assumenda temporibus consequuntur alias debitis magnam eum
              consequatur magni. Suscipit amet mollitia accusantium, quod asperiores eaque libero vel rerum, neque
              possimus laborum, dolor totam reprehenderit aspernatur. Aspernatur eius iste dicta, odio ipsam
              consectetur, tempore quis praesentium expedita sed aliquid!
            </p>
            <p class="mt-[120px]">
              <span class="font-[mersb] text-[28px] mb-[10px] block">Another one Mercedes-Benz.</span> <br>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium rem recusandae sequi nam nesciunt
              earum maxime et sapiente a dicta facilis quae quam, ducimus incidunt quis magnam voluptatibus accusamus
              dolor odit iste quibusdam eligendi dolorem accusantium. Dignissimos qui fuga non, totam, nobis nisi
              aperiam veritatis blanditiis tempore et odit commodi magni laboriosam animi dicta. Rerum assumenda
              accusantium ab voluptas odit laudantium eveniet similique molestias sed, maxime quis ad numquam ratione.
              Ipsum repudiandae, optio debitis reiciendis iste dolores aperiam perspiciatis quibusdam, exercitationem
              sint doloremque velit culpa impedit repellendus, quia quod quisquam hic libero? Minus dolorum ullam
              tenetur ad enim illum explicabo tempora, assumenda temporibus consequuntur alias debitis magnam eum
              consequatur magni. Suscipit amet mollitia accusantium, quod asperiores eaque libero vel rerum, neque
              possimus laborum, dolor totam reprehenderit aspernatur. Aspernatur eius iste dicta, odio ipsam
              consectetur, tempore quis praesentium expedita sed aliquid!
            </p>

          </div>
        </div>
      </section>
      <div class="h-[50vh]"></div>
    </main>
  </div>
</template>

<style scoped>
.header{
  transition-duration: .3s;
}
.activeheader{
  height: 70px;
  backdrop-filter: blur(10px);
  background: black;
}
.imgimg {
  background-image: url('https://klassen.de/media/images/home/makes/V-Class.jpg');
  background-repeat: no-repeat;
  background-position: 245px 180px;
  background-size: 700px;
  background-attachment: fixed;
}
.imgimg3 {
  background-image: url('https://klassen.de/media/images/home/makes/V-Class.jpg');
  background-repeat: no-repeat;
  background-position: 245px 180px;
  background-size: 700px;
  background-attachment: fixed;
}
.imgimg2 {
  background-image: url('https://klassen.de/media/images/home/makes/Sprinter-VIP.jpg?v=2');
  background-repeat: no-repeat;
  background-position: 245px 180px;
  background-size: 700px;
  background-attachment: fixed;
}

.first::after {
  content: "";
  position: absolute;
  left: 0;
  width: 100%;
  top: 0;
  height: 100%;
  background: rgba(0, 0, 0, 0.886);
}

.hoverblock {
  transition-duration: .2s;
  position: absolute;
  transform: translateY(70px);
}

.removeblock {
  transition-duration: .3s;
}

.hoveritems::after {
  content: '';
  position: absolute;
  left: 0;
  width: 100%;
  height: 100%;
  bottom: -100%;
  transition-duration: .3s;
  z-index: -1;
  background: rgb(23, 23, 23);
}

.hoveritems {
  z-index: 1;
  cursor: pointer;
  overflow: hidden;
  position: relative;
}

.hoveritem {
  cursor: pointer;
  overflow: hidden;
  position: relative;
}

.hoveritem:hover .hoverblock {
  transform: translateY(0px);
}

.hoveritem:hover .removeblock {
  transform: translateY(-70px);
}

.hoveritems:hover::after {
  bottom: 0px;
}



.searcher::after {
  content: '';
  position: absolute;
  left: 0;
  width: 100%;
  height: 100%;
  bottom: -100%;
  transition-duration: .3s;
  z-index: -1;
  background: rgb(218, 218, 218);
}

.searcher {
  z-index: 1;
  cursor: pointer;
  overflow: hidden;
  position: relative;
}

.searcher:hover::after {
  bottom: 0px;
}
</style>
