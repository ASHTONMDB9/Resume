<template>
    <h1 id="Art">Gallery</h1>

    <div class="container-fluid mt-5">
<div v-for="Artwork of Artworks" :key="Artworks.id">
<div id="gallery" class="card text-light mt-3 mb-2 ms-2 me-2">
    <img id="work" v-bind:src="Artwork.image" class="card-img" style="height: 40rem; object-fit: cover;">
    <h4 class="caption">{{ Artwork.name }}</h4>
    </div>
</div>
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
    .card {
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
    }
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