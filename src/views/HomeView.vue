<template>
  <div class="flex flex-col mx-16">
    <NavBar/>

    <section class="flex flex-col items-center pt-36 pb-10">
      <div class=" flex flex-col gap-1 items-start mx-auto w-7/12 text-left"> 
        <h1 class="text-7xl font-bold text-blue-600">A design conference for the dark side.</h1>
        <p class="text-blue-800 text-2xl leading-10 tracking-tight mt-6">The next generation of web users are tech-savvy and suspicious. They know how to use dev tools, they can detect a phishing scam from a mile away, and they certainly aren’t accepting any checks from Western Union.</p>
        <p class="text-blue-800 text-2xl leading-10 tracking-tight mt-4" >At DeceptiConf you’ll learn about the latest dark patterns being developed to trick even the smartest visitors, and you’ll learn how to deploy them without ever being detected.</p>
      </div>
      <div class="flex justify-between pr-3 w-7/12 mt-10">
        <div class="text-left">
          <span class="text-sm leading-6 text-blue-600 font-mono font-semibold ">Speakers</span>
          <p class="text-2xl text-blue-900 font-semibold tracking-tight " >18</p>
        </div>
        <div class="text-left">
          <span class="text-sm leading-6 text-blue-600 font-mono font-semibold">People Attending</span>
          <p class="text-2xl text-blue-900 font-semibold tracking-tight">2,091</p>
        </div>
        <div class="text-left">
          <span class="text-sm leading-6 text-blue-600 font-mono font-semibold ">Venue</span>
          <p class="text-2xl text-blue-900 font-semibold tracking-tight ">Staples Center</p>
        </div>
        <div class="text-left">
          <span class="text-sm leading-6 text-blue-600 font-mono font-semibold">Location</span>
          <p class="text-2xl text-blue-900 font-semibold tracking-tight ">Los Angeles</p>
        </div>
      </div>
    </section>

    <section class="flex flex-col items-start text-left pt-36 w-3/6" >
      <h3 class="text-4xl font-semibold text-blue-600">Speakers</h3>
      <p class="text-blue-800 text-2xl leading-10 tracking-tight mt-3 ">Learn from the experts on the cutting-edge of deception at the most sinister companies.</p>
    </section>
    
    <section class="flex justify-between mt-36 ">
      <div class="flex flex-col items-start h-auto text-left" >
        <div class="pl-6 border-l-2 border-double border-slate-500">
          <span class="text-sm leading-6 text-blue-600 font-mono font-semibold ">Opening Day</span>
          <p class="text-2xl text-blue-900 font-semibold tracking-tight mb-8" >April 4</p>
        </div>
        <br>
        <div class="pl-6 border-l-2 border-double border-slate-500" >
          <span class="text-sm leading-6 text-blue-600 font-mono font-semibold ">Speakers & Workshops</span>
          <p class="text-2xl text-blue-900 font-semibold tracking-tight mb-8" >April 5</p>
        </div>
        <br>
        <div class="pl-6 border-l-2 border-double border-slate-500"  >
          <span class="text-sm leading-6 text-blue-600 font-mono font-semibold ">Interviews</span>
          <p class="text-2xl text-blue-900 font-semibold tracking-tight mb-8" >April 6</p>
        </div>
      </div>
      <div class="grid grid-cols-3 gap-3" >
        <div v-for="card in this.cards" :key="card" class="my-3">
          <img class="rounded-3xl" :src="card.img" alt="img">
          <h2 class="font-bold text-xl mt-8" >{{  card.title  }}</h2>
          <span class=" pt-1 text-base tracking-tight text-slate-500" >{{ card.disc }}</span>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import NavBar from '@/components/NavBar.vue';

export default {
  name: 'HomeView',
  components: {
    NavBar
  },
  data() {
    return {
    cards : [
      {
        img: "https://source.unsplash.com/featured/300x201",
        title: 'Steven McHail',
        disc: 'Designer at Globex Corporation'
      },
      {
        img: "https://source.unsplash.com/featured/300x201",
        title: 'Steven McHail',
        disc: 'Designer at Globex Corporation'
      },
      {
        img: "https://source.unsplash.com/featured/300x201",
        title: 'Steven McHail',
        disc: 'Designer at Globex Corporation'
      },
      {
        img: "https://source.unsplash.com/featured/300x201",
        title: 'Steven McHail',
        disc: 'Designer at Globex Corporation'
      },
      {
        img: "https://source.unsplash.com/featured/300x201",
        title: 'Steven McHail',
        disc: 'Designer at Globex Corporation'
      },
      {
        img: "https://source.unsplash.com/featured/300x201",
        title: 'Steven McHail',
        disc: 'Designer at Globex Corporation'
      }
    ]
    }
  }
}
</script>
