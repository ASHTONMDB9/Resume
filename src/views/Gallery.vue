<template>
    <h1 id="Art">Gallery</h1>
    <p class="d-flex justify-content-center align-items-center text-white">Hover over each image to view</P>
    <div class="container-fluid mt-5 mb-5">
      <div class="container">
	<div class="box box-1" style="--img: url(https://i.postimg.cc/9Qm4vWBt/20230117-094055.jpg);" loading="lazy" data-text="Itachi of the Sharingan"></div>
	<div class="box box-2" style="--img: url(https://i.postimg.cc/Bn7vk2b4/20230117-094125.jpg);" loading="lazy" data-text="The Terrifying Androids"></div>
	<div class="box box-3" style="--img: url(https://i.postimg.cc/gc3njwSH/20230117-094140.jpg);" loading="lazy" data-text="The Victoria"></div>
	<div class="box box-4" style="--img: url(https://i.postimg.cc/28m3ZzgR/20230117-094149.jpg);" loading="lazy" data-text="Pan, Daughter of Gohan"></div>
	<div class="box box-5" style="--img: url(https://i.postimg.cc/QMBM3VK5/20230117-094157.jpg);" loading="lazy" data-text="Sunshine"></div>
  <div class="box box-6" style="--img: url(https://i.postimg.cc/G2Gh4NQm/20230117-094211.jpg);" loading="lazy" data-text="Rivals Unite"></div>
  <div class="box box-7" style="--img: url(https://i.postimg.cc/ydms1R1J/20230117-094249.jpg);" loading="lazy" data-text="I Heart Eren Jaeger"></div>
  <div class="box box-8" style="--img: url(https://i.postimg.cc/4ywGtThs/20230117-094258.jpg);" loading="lazy" data-text="The warrior of Hope"></div>
  <div class="box box-9" style="--img: url(https://i.postimg.cc/vTGMcmT0/20230117-094307.jpg);" loading="lazy" data-text="Summertime Sadness"></div>
  <div class="box box-10" style="--img: url(https://i.postimg.cc/nzbnf2Jb/20230117-094320.jpg);" loading="lazy" data-text="The Hopes and Dreams of One Sir Alex"></div>
  <div class="box box-11" style="--img: url(https://i.postimg.cc/J46mzMLQ/20230117-094346.jpg);" loading="lazy" data-text="The Almighty Prince Vegeta"></div>
  <div class="box box-12" style="--img: url(https://i.postimg.cc/Hssdmjfx/20230117-094356.jpg);" loading="lazy" data-text="He Who Once Was"></div>
  <div class="box box-13" style="--img: url(https://i.postimg.cc/0Q01RqnD/20230117-094407.jpg);" loading="lazy" data-text="What Is That Mellow-dy?"></div>
  <div class="box box-14" style="--img: url(https://i.postimg.cc/j28V2QGj/20230117-094419.jpg);" loading="lazy" data-text="I Don't Need The Blood Stains To Match My Eyes"></div>
  <div class="box box-15" style="--img: url(https://i.postimg.cc/3r9QtYdH/20230117-094429.jpg);" loading="lazy" data-text="The Angel Born In Hell"></div>
  <div class="box box-16" style="--img: url(https://i.postimg.cc/SxBBnKtc/20230117-094456.jpg);" loading="lazy" data-text="The Dragon Sin of Wrath"></div>
  <div class="box box-17" style="--img: url(https://i.postimg.cc/g0tsGQCw/20230117-094113.jpg);" loading="lazy" data-text="The Japanese Dream"></div>
  <div class="box box-18" style="--img: url(https://i.postimg.cc/kGKvF4B8/20230117-094133.jpg);" loading="lazy" data-text="Miniture Victory"></div>
  <div class="box box-19" style="--img: url(https://i.postimg.cc/Kv7511Xh/20230117-094224.jpg);" loading="lazy" data-text="The Ultimate Power"></div>
  <div class="box box-20" style="--img: url(https://i.postimg.cc/wj6QL9Hy/20230117-094237.jpg);" loading="lazy" data-text="Alex Goes Down The Rabbit Hole"></div>
  <div class="box box-21" style="--img: url(https://i.postimg.cc/hPRr4950/20230117-094330.jpg);" loading="lazy" data-text="Classy and Comfortable"></div>
  <div class="box box-22" style="--img: url(https://i.postimg.cc/G3yK1Mq2/20230117-094443.jpg);" loading="lazy" data-text="Love Is Blind, Deaf and Dumb"></div>
</div>
<!-- <div v-for="Artwork of Artworks" :key="Artworks.id">
<div id="gallery" class="card text-light mt-3 mb-2 ms-2 me-2">
    <img id="work" v-bind:src="Artwork.image" class="card-img" style="height: 40rem; object-fit: cover;">
    <h4 class="caption">{{ Artwork.name }}</h4>
    </div>
</div> -->
</div>
<div>
    <router-link to="/About"><button class="work w-100"><h6>Back</h6></button></router-link>
</div>
    
    </template>
    <script>
    export default {
        data() {
        return {
           Artworks : [
          {
            id: "1",
            image: "https://i.postimg.cc/9Qm4vWBt/20230117-094055.jpg",
            name: "Itachi of the Sharingan",
          },
          {
            id: "2",
            image: "https://i.postimg.cc/Bn7vk2b4/20230117-094125.jpg",
            name: "The Terrifying Androids",
          },
          {
            id: "3",
            image: "https://i.postimg.cc/gc3njwSH/20230117-094140.jpg",
            name: "The Victoria",
          },
          {
            id: "4",
            image: "https://i.postimg.cc/28m3ZzgR/20230117-094149.jpg",
            name: "Pan, Daughter of Gohan",
          },
          {
            id: "5",
            image: "https://i.postimg.cc/QMBM3VK5/20230117-094157.jpg",
            name: "Sunshine",
          },
          {
            id: "6",
            image: "https://i.postimg.cc/G2Gh4NQm/20230117-094211.jpg",
            name: "Rivals Unite",
          },
          {
            id: "7",
            image: "https://i.postimg.cc/ydms1R1J/20230117-094249.jpg",
            name: "I Heart Eren Jaeger",
          },
          {
            id: "8",
            image: "https://i.postimg.cc/4ywGtThs/20230117-094258.jpg",
            name: "The warrior of Hope",
          },
          {
            id: "9",
            image: "https://i.postimg.cc/vTGMcmT0/20230117-094307.jpg",
            name: "Summertime Sadness",
          },
          {
            id: "10",
            image: "https://i.postimg.cc/nzbnf2Jb/20230117-094320.jpg",
            name: "The Hopes and Dreams of One Sir Alex",
          },
          {
            id: "11",
            image: "https://i.postimg.cc/J46mzMLQ/20230117-094346.jpg",
            name: "The Almighty Prince Vegeta",
          },
          {
            id: "12",
            image: "https://i.postimg.cc/Hssdmjfx/20230117-094356.jpg",
            name: "He Who Once Was",
          },
          {
            id: "13",
            image: "https://i.postimg.cc/0Q01RqnD/20230117-094407.jpg",
            name: "What Is That Mellow-dy",
          },
          {
            id: "14",
            image: "https://i.postimg.cc/j28V2QGj/20230117-094419.jpg",
            name: "I Don't Want The Blood Stains To Match My Eyes",
          },
          {
            id: "15",
            image: "https://i.postimg.cc/3r9QtYdH/20230117-094429.jpg",
            name: "The Angel Born In Hell",
          },
          {
            id: "16",
            image: "https://i.postimg.cc/SxBBnKtc/20230117-094456.jpg",
            name: "The Dragon Sin of Wrath",
          },
          {
            id: "17",
            image: "https://i.postimg.cc/g0tsGQCw/20230117-094113.jpg",
            name: "The Japanese Dream",
          },
          {
            id: "18",
            image: "https://i.postimg.cc/kGKvF4B8/20230117-094133.jpg",
            name: "Miniture Victory",
          },
          {
            id: "19",
            image: "https://i.postimg.cc/Kv7511Xh/20230117-094224.jpg",
            name: "The Ultimate Power",
          },
          {
            id: "20",
            image: "https://i.postimg.cc/wj6QL9Hy/20230117-094237.jpg",
            name: "Alex Goes Down The Rabbit Hole",
          },
          {
            id: "21",
            image: "https://i.postimg.cc/hPRr4950/20230117-094330.jpg",
            name: "Classy and Comfortable",
          },
          {
            id: "22",
            image: "https://i.postimg.cc/G3yK1Mq2/20230117-094443.jpg",
            name: "Love Is Blind, Deaf and Dumb",
          }
          
        ] 
    }
        }
    }
    </script>

    <style scoped>
    * {
        padding: 0;
        margin: 0;
    }
    body {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    #Art {
       color: white;
       margin-top: 80px;
       text-align: center;
       text-decoration: underline 3px;
       text-decoration-color: blue;
    }
    .container-fluid {
       display: flex;
       flex-wrap: wrap;
       justify-content: space-evenly;
       align-items: center;
    }


/* body {
	display: grid;
	place-content: center;
	min-height: 100vh;
	background: #000;
} */

.container {
	display: grid;
	grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr;
	gap: 1em;
	width: 800px;
	height: 500px;
	transition: all 400ms;
}

.container:hover .box {
	filter: grayscale(100%) opacity(24%);
}

.box {
	position: relative;
	background: var(--img) center center;
	background-size: cover;
	transition: all 400ms;
	display: flex;
	justify-content: center;
	align-items: center;
}

.container .box:hover {
	filter: grayscale(0%) opacity(100%);
}

.container:has(.box-1:hover) {
	grid-template-columns: 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-2:hover) {
	grid-template-columns: 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-3:hover) {
	grid-template-columns: 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-4:hover) {
	grid-template-columns: 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-5:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-6:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-7:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-8:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-9:hover) {
  grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-10:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-11:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-12:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-13:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-14:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-15:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-16:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-17:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-18:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr 10fr;
}

.container:has(.box-19:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr 10fr;
}

.container:has(.box-20:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr 10fr;
}

.container:has(.box-21:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr 10fr;
}

.container:has(.box-22:hover) {
	grid-template-columns: 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 10fr 500fr;
}

.box:nth-child(odd) {
	transform: translateY(-16px);
}

.box:nth-child(even) {
	transform: translateY(16px);
}

.box::after {
	content: attr(data-text);
	position: absolute;
	bottom: 20px;
	background: #000;
	color: blue;
	padding: 10px 10px 10px 14px;
	letter-spacing: 4px;
	text-transform: uppercase;
	transform: translateY(60px);
	opacity: 0;
	transition: all 400ms;
}

.box:hover::after {
	transform: translateY(0);
	opacity: 1;
	transition-delay: 400ms;
}

    /* .card {
       display: inline-block;
       position: relative;
       height: 40rem;
       width: 3rem;
       border-radius: 10px;
       overflow: hidden;
       transition: 0.5s;
    }

    .card:hover {
       width: 28rem;
    }
    .card:hover .caption {        
       opacity: 1;
       bottom: 0;
}
    .caption {
        text-decoration: underline 3px;
        text-decoration-color: blue;
        position: absolute;
        z-index: 2;
        bottom: -20px;
        width: 100%;
        color: white;
        padding-bottom: 15px;
        padding-top: 10px;
        background: rgb(0,0,0);
        background: linear-gradient(0deg, rgba(0,0,0,1) 0%, rgba(8,8,8,1) 57%, rgba(255,255,255,0) 100%);
        opacity: 0;
        transition-delay:0.2s;
        transition-duration: 1s;
    }*/
    .work {
        color: blue;
        height: 50px;
        background-color: black;
        border: 1px solid blue;
    }
    .work:hover {
        color: black;
        background-color: white;
        border: 1px solid black;
    }
    @media only screen and (max-width: 1200px){
        .card {
            min-width: 30rem;
    }
   }
    @media only screen and (max-width: 600px){
        .card {
            min-width: 25rem;
            height: 40rem;
    }
   }
    @media only screen and (max-width: 425px){
        .card {
            height: 35rem;
            min-width: 19rem;
    }
   }
</style> 