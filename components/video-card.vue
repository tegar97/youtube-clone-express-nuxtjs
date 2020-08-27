<template>
<nuxt-link to="/watch/tes">
    <div class="card">
        <figure class="thumbnail">
                
               <img src="./../assets/image/thumbnail.jpg" alt="" class="card__thumbnail">
               <div class="d-flex justify-content-end card-time">
                        <figcaption class="card__duration">9.32</figcaption>


               </div>
               <div class="row card-body   ">
                    <div class="col-3 col-lg-2">
                       <img src="./../assets/image/profile.jpg" class="card__channel-image">
                    </div>
                    <div class="col-9 col-lg-10">
                         <div class="card__text">
                  
                   
                            <span class="card__text-title">GTA V MOD  GRAPICH </span>
                            <span class="card__text-channel">Tegar </span>
                            <span class="card__text-views">100 rb x ditonton . </span>
                            <span class="card__text-date">Streaming 1 minggu yang lalu </span>
                        
                         </div>

                    </div>
               </div>
              
           
              
        </figure>
     
    </div>

</nuxt-link>
</template>

<style lang="scss" scoped>
.card{
    border: none !important;
       position: relative;
       background: transparent;
    &__thumbnail{
        width: 100%;
        height: 20rem;
     
        
    }
    &-body{
        padding: 0;
        margin-top: 3rem !important;
    }
    
    
    &__duration{
     
        background: black;
        position: absolute;
        font-size: 1.4rem;
        opacity: 80%;
        font-weight: 500;
        padding: 0 1rem;
        color: #fff;
           
        
        
    }
    &__channel-image{
          width: 4rem;
        border-radius: 100%;

    }
    &__text{
        display: flex;
        flex-direction: column;
        color: #aaa;
        font-weight: 400;
        font-size: 1.45rem;

        &-title{
            font-size: 1.5rem;
            font-weight: 600;
            line-height: 1.7;
            color: #fff;
        
        }
    }
    &:hover{
        
    }
}
.card::after{

}
.card-time{
    margin-left: 1rem;
    align-items: center;
    margin-top: -2rem;
    margin-right: 1rem;

 
}
</style>