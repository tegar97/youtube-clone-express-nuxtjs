<template>

    <div>
  
       <div class="container mt-5 ">
           
           <div class="row ">
              <div class="video-container">
                <iframe autoplay width="100%" height="500" class="video" allow='autoplay' src="https://www.youtube.com/embed/qHer-rGfTco?autoplay=1">
                </iframe>
                <div class="hastag">
                  <a class="video-hastag mt-2 ">#reddead2</a>
                  <a class="video-hastag mt-2 ml-2">#reddead2</a>
                </div>

                <h1 class="video-title mt-2">Red Dead Redemption 2 Official Soundtrack - See The Fire In Your Eyes | HD
                  (With Visualizer)</h1>
                <div class="video-info">
                    <span class="video-views ">1.927.288 x ditonton</span>
                    <span class="video-date ml-2">•19 Jan 2014</span>
                    <div class="video-info-right">
                        <a v-on:click="sumLike(); isLike = !isLike; " ><i class="fas fa-thumbs-up" :class="{active : isLike}"></i><span class="ml-3" :class="{active : isLik}" >{{like}} </span> </a>
                        <a v-on:click="sumDislike(); isDislike = !isDislike;"><i class="fas fa-thumbs-down ml-5" :class="{active : isDislike}"></i><span class="ml-3" >{{dislike}}</span></a>
                        <span><i class="fas fa-share ml-5"></i> <span class="ml-3">Bagikan</span></span>
                        <span><i class="fas fa-save ml-5"></i> <span class="ml-3">Simpan</span></span>
                        <span><i class=" fas fa-ellipsis-h ml-5"></i></span>

                    </div>
                 
                </div>
                <div class="line mt-4"></div>
                <div class="video-description mt-5">
                    <img src="./../../assets/image/profile.jpg" alt="profile " class="channel-image mt-2">
                    <div class="channel-info ml-5 mr-auto">
                        <span class="channel-name ">Tegar Akmal</span>
                        <span class="text-secondary-2 mr-auto">29,6 rb subscriber</span>
                        
                        

                    </div>
                    <div class="subscribe">
                        <button class="btn-subscribe " v-on:click="isSubscribe = !isSubscribe " v-if="!isSubscribe">subscribe</button>
                        <button class="btn-subscribe btn-active" v-on:click="isSubscribe = !isSubscribe " v-if="isSubscribe">Di Subscribe</button>
                            <i class="fas fa-bell ml-4" v-if="isSubscribe" style="font-size: 2.4rem; color: #fff;"></i>

                    </div>
                </div>
                    <div class="description-box  mt-5">
                         <p class="description">What is Lorem Ipsum?
                           Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has
                           been the industry's standard dummy text ever since the 1500s,<br> when an unknown printer took a
                           galley of type and scrambled it to make a type specimen book. It has survived not only five
                           centuries, <br>but also the leap into electronic typesetting, remaining essentially unchanged. It
                           was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum
                           passages,<br> and more recently with desktop publishing software like Aldus PageMaker including
                           versions of Lorem Ipsum.

                          
                            </p>
                    </div>
                      <div class="line mt-4"></div>
                    <section class="section-komentar">
                        <div class="komentar-data mt-3">
                          <span class="text-white ">230 Komentar</span>
                          <span class="text-secondary-2 ml-5"><i class="fas fa-sort-amount-down"></i>Urutkan</span>
                        
                        </div>
                          <div class="komentar-input mt-5">
                                <img src="./../../assets/image/profile.jpg" alt="profile " class="channel-image mt-2">
                               

                       
                                <input placeholder="komentar anda disini    " class="form-input ml-3" v-on:click="Iscommentary = true">
                               
                          </div>
                           <div class="komentar-button">
                                 <button class="btn btn-transparent btn-lg ml-3 text-white" v-on:click="Iscommentary = false" v-if="Iscommentary">Batal</button> 
                                 <button class="btn btn-secondary btn-lg" v-if="Iscommentary">Submit</button>

                            </div>
                                
                    </section>
                    <br>
              </div>
                   

         
             VIDEO CARD
           </div>
       </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            isSubscribe: false,
            isLike: false,
            isDislike: false,
            like: 0,
            dislike: 0,
            Iscommentary: false
        }
    },
    computed:{},
    methods:{
        sumLike() {
            if(this.isLike) {
                 this.like -= 1
              
            }else if(!this.isLike){
                  this.like += 1
            }
        },
        sumDislike() {
            if(this.isDislike) {
                 this.dislike -= 1
              
            }else if(!this.isDislike){
                  this.dislike += 1
            }
        }
    }
}
</script>
<style lang="scss" scoped>
.video-container{
    display: flex;
    flex-direction: row;
    margin-left: -11rem;
    flex-basis: 85%;
    flex-direction: column;
}
.video{
    border: none;

    &-hastag{
        font-size: 1.8rem
    }
   
}
.video-title{
    font-size: 2.3rem;
    font-weight: 400;
    text-align: left;
}
.hastag{
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    
}
.video-info{
    display: flex;
    font-size: 1.8rem;
    color: #aaa;
    


    &-right{
        margin-right: 1rem;
          
    }

}
.video-date{
    margin-right: auto;
}
.video-description{
    display: flex;
    flex-direction: row;
}
.line{
    border-bottom: 1px solid #aaa;
    opacity: 30%;
}
.channel-image{
          width: 4rem;
          height: 4rem;
        border-radius: 100%;
}
.channel-info{
    display: flex;
    flex-direction: column;
}
.subscribe{
    display: flex;
    align-items: center;
}
.active{
    color: #3ea6ff;

}
.description-box{
    width: 80%;
    margin-left: 7rem;
}
.description{
    font-size: 1.5rem;
    font-weight: 400;
}
.komentar-data{
    display: flex;
    flex-direction: row;
    align-items: center;
    span{
        font-size: 2rem;;
        font-weight: 400;
    }
   
}
.komentar{
    &-input{
            display: flex;
    align-items: flex-start;
    }
    &-button{
        display: flex;
        flex-direction: row;
        justify-content: flex-end;
    }
}


.form-input{
    width: 100%;
    background-color: #191919;
    color: #fff;
    font-size: 2rem;
    padding: .2rem 1rem;
    border: none;
    border-bottom: 1px solid #aaa;
    transition: all .3s ease-in;
    

    &:focus{
        outline: none;
            border-bottom: 1px solid black;
    }
}
</style>