<template>
    <div>
       <div class="container mt-5 ">
           <div class="row ">
              <div class="video-container">
                <iframe width="100%" height="500" class="video" src="https://www.youtube.com/embed/qHer-rGfTco">
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
                        <span><i class="fas fa-thumbs-up"></i><span class="ml-3">21 rb</span> </span>
                        <span><i class="fas fa-thumbs-down ml-5"></i><span class="ml-3">12</span></span>
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
            isSubscribe: false
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
</style>