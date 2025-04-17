<template>
    <h1 id="Art">Gallery</h1>
    <p class="d-flex justify-content-center align-items-center text-white">Hover over each image to view</P>
      <p class="d-flex justify-content-center align-items-center text-white">A few of the works I've done in my spare time</P>
    <div class="container-fluid mt-5 mb-5">
      <div class="container">
	<div class="box box-1" style="--img: url(https://i.postimg.cc/BQ9qkJ7s/Itachi.jpg);" loading="lazy" data-text="Itachi of the Sharingan"></div>
	<div class="box box-2" style="--img: url(https://i.postimg.cc/Ls1cS1bs/Androids.jpg);" loading="lazy" data-text="The Terrifying Androids"></div>
	<div class="box box-3" style="--img: url(https://i.postimg.cc/d3HHrsxX/Victoria.jpg);" loading="lazy" data-text="The Victoria"></div>
	<div class="box box-4" style="--img: url(https://i.postimg.cc/KzxWBsJ6/Pan.jpg);" loading="lazy" data-text="Pan, Daughter of Gohan"></div>
	<div class="box box-5" style="--img: url(https://i.postimg.cc/nLv5stYK/Muminah.jpg);" loading="lazy" data-text="Sunshine"></div>
  <div class="box box-6" style="--img: url(https://i.postimg.cc/tJCvsZ2W/Vegito.jpg);" loading="lazy" data-text="Rivals Unite"></div>
  <div class="box box-7" style="--img: url(https://i.postimg.cc/HW2fTHBb/Levi.jpg);" loading="lazy" data-text="I Heart Eren Jaeger"></div>
  <div class="box box-8" style="--img: url(https://i.postimg.cc/NF0PP2hb/Trunks.jpg);" loading="lazy" data-text="The warrior of Hope"></div>
  <div class="box box-9" style="--img: url(https://i.postimg.cc/pTQ3htxb/Issues.jpg);" loading="lazy" data-text="Summertime Sadness"></div>
  <div class="box box-10" style="--img: url(https://i.postimg.cc/YChcXVNY/Dreams.jpg);" loading="lazy" data-text="The Hopes and Dreams of One Sir Alex"></div>
  <div class="box box-11" style="--img: url(https://i.postimg.cc/yxFzsSpK/vegeta.jpg);" loading="lazy" data-text="The Almighty Prince Vegeta"></div>
  <div class="box box-12" style="--img: url(https://i.postimg.cc/cLjpPmTj/Alex.jpg);" loading="lazy" data-text="He Who Once Was"></div>
  <div class="box box-13" style="--img: url(https://i.postimg.cc/FHfqbSmx/Marshmellow.jpg);" loading="lazy" data-text="What Is That Mellow-dy?"></div>
  <div class="box box-14" style="--img: url(https://i.postimg.cc/d1FxKSCW/Obtio.jpg);" loading="lazy" data-text="I Don't Need The Blood Stains To Match My Eyes"></div>
  <div class="box box-15" style="--img: url(https://i.postimg.cc/W38Hn6yh/Gogeta.jpg);" loading="lazy" data-text="The Angel Born In Hell"></div>
  <div class="box box-16" style="--img: url(https://i.postimg.cc/1zwj2Z8n/Meliodas.jpg);" loading="lazy" data-text="The Dragon Sin of Wrath"></div>
  <div class="box box-17" style="--img: url(https://i.postimg.cc/0QCH5dd9/Skyline.jpg);" loading="lazy" data-text="The Japanese Dream"></div>
  <div class="box box-18" style="--img: url(https://i.postimg.cc/YCJPdSCB/Mini.jpg);" loading="lazy" data-text="Miniture Victory"></div>
  <div class="box box-19" style="--img: url(https://i.postimg.cc/gJbf22CH/Gohan.jpg);" loading="lazy" data-text="The Ultimate Power"></div>
  <div class="box box-20" style="--img: url(https://i.postimg.cc/Fz980nsf/Kirito.jpg);" loading="lazy" data-text="Alex Goes Down The Rabbit Hole"></div>
  <div class="box box-21" style="--img: url(https://i.postimg.cc/ZnVgHFCw/Land-Rover.jpg);" loading="lazy" data-text="Classy and Comfortable"></div>
  <div class="box box-22" style="--img: url(https://i.postimg.cc/Kv8CzVHw/Love.jpg);" loading="lazy" data-text="Love Is Blind, Deaf and Dumb"></div>
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
            image: "https://i.postimg.cc/BQ9qkJ7s/Itachi.jpg",
            name: "Itachi of the Sharingan",
          },
          {
            id: "2",
            image: "https://i.postimg.cc/Ls1cS1bs/Androids.jpg",
            name: "The Terrifying Androids",
          },
          {
            id: "3",
            image: "https://i.postimg.cc/d3HHrsxX/Victoria.jpg",
            name: "The Victoria",
          },
          {
            id: "4",
            image: "https://i.postimg.cc/KzxWBsJ6/Pan.jpg",
            name: "Pan, Daughter of Gohan",
          },
          {
            id: "5",
            image: "https://i.postimg.cc/nLv5stYK/Muminah.jpg",
            name: "Sunshine",
          },
          {
            id: "6",
            image: "https://i.postimg.cc/tJCvsZ2W/Vegito.jpg",
            name: "Rivals Unite",
          },
          {
            id: "7",
            image: "https://i.postimg.cc/HW2fTHBb/Levi.jpg",
            name: "I Heart Eren Jaeger",
          },
          {
            id: "8",
            image: "https://i.postimg.cc/NF0PP2hb/Trunks.jpg",
            name: "The warrior of Hope",
          },
          {
            id: "9",
            image: "https://i.postimg.cc/pTQ3htxb/Issues.jpg",
            name: "Summertime Sadness",
          },
          {
            id: "10",
            image: "https://i.postimg.cc/YChcXVNY/Dreams.jpg",
            name: "The Hopes and Dreams of One Sir Alex",
          },
          {
            id: "11",
            image: "https://i.postimg.cc/yxFzsSpK/vegeta.jpg",
            name: "The Almighty Prince Vegeta",
          },
          {
            id: "12",
            image: "https://i.postimg.cc/cLjpPmTj/Alex.jpg",
            name: "He Who Once Was",
          },
          {
            id: "13",
            image: "https://i.postimg.cc/FHfqbSmx/Marshmellow.jpg",
            name: "What Is That Mellow-dy",
          },
          {
            id: "14",
            image: "https://i.postimg.cc/d1FxKSCW/Obtio.jpg",
            name: "I Don't Need The Blood Stains To Match My Eyes",
          },
          {
            id: "15",
            image: "https://i.postimg.cc/W38Hn6yh/Gogeta.jpg",
            name: "The Angel Born In Hell",
          },
          {
            id: "16",
            image: "https://i.postimg.cc/1zwj2Z8n/Meliodas.jpg",
            name: "The Dragon Sin of Wrath",
          },
          {
            id: "17",
            image: "https://i.postimg.cc/0QCH5dd9/Skyline.jpg",
            name: "The Japanese Dream",
          },
          {
            id: "18",
            image: "https://i.postimg.cc/YCJPdSCB/Mini.jpg",
            name: "Miniture Victory",
          },
          {
            id: "19",
            image: "https://i.postimg.cc/gJbf22CH/Gohan.jpg",
            name: "The Ultimate Power",
          },
          {
            id: "20",
            image: "https://i.postimg.cc/Fz980nsf/Kirito.jpg",
            name: "Alex Goes Down The Rabbit Hole",
          },
          {
            id: "21",
            image: "https://i.postimg.cc/ZnVgHFCw/Land-Rover.jpg",
            name: "Classy and Comfortable",
          },
          {
            id: "22",
            image: "https://i.postimg.cc/Kv8CzVHw/Love.jpg",
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
	color: blue;
  background: rgb(0, 0, 0, 0.4);
	padding: 10px 10px 10px 14px;
	letter-spacing: 4px;
	text-transform: uppercase;
  font-weight: bold;
  text-shadow: 2px 2px 3px black;
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