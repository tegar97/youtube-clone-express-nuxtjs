<template>
      <div class="header">
       
        <div class="header__logo">
        <svg class="icon icon-home header__logo-icon"><use xlink:href="./../assets/image/symbol-defs.svg#icon-menu" ></use></svg>
            <img src="./../assets/image/yt_logo_rgb_dark.png" class="logo ml-5">
        </div>
        <form action="#" class="header__search">
          <input placeholder="Telusuri" class="header__search-bar">
          <!-- <button class="btn btn--secondary--costume">
                      <svg class="icon icon-search header__search-icon"><use xlink:href="./../assets/image/symbol-defs.svg#icon-search" ></use></svg>

          </button> -->
        </form>
        <div class="user-nav">
           <div class="user-nav__icon-box">
                    <svg class="user-nav__icon">
                        <use xlink:href="./../assets/image/symbol-defs.svg#icon-video-camera  "></use>
                    </svg>
                   
             </div>
           <div class="user-nav__icon-box">
                    <svg class="user-nav__icon">
                        <use xlink:href="./../assets/image/symbol-defs.svg#icon-bell"></use>
                    </svg>
                    <span class="user-nav__bell">9+</span>
             </div>
             <div class="user-nav__icon-box">
                 <img src="./../assets/image/profile.jpg" class="user-photo">
             </div>
          
        </div>
    </div>
</template>
<style lang="scss" scoped>
.header{
  display: flex;
  background-color: #262626;
  height: 5.6rem;
  justify-content: space-between;
  align-items: center;
  &__logo{
    margin-left: 3rem;

    &-icon{
      width: 3rem;
     height: 3rem;
      fill: #fff;
      
      
    }
  }
}

.logo{
  width: 100px;
  
}

.header__search{
    display: flex;
    flex: 0 0 40%;
    align-items: center;
    justify-content: center;
  &-bar{
    font-size: 1.9rem;
    padding: 0 1rem;
    margin-left: -21rem;
    width: 100%;
    border: 1px solid #303030;
    background-color: #191919;
    color: #ffff;
 
    
    &:focus {
      border: 1px solid blue !important;
    }
      &::-webkit-input-placeholder{
          font-weight: 400;
           color: #636363 !important;
    }
  
  }
 
 
}
.header__search-icon{
 
  width: 1.5rem;
  height: 1.5rem;
  fill: #fff;

  

  
  
}
.header__user{
  margin-right: 2rem;
}
.user-photo{
  width: 4rem;
  border-radius: 100%;

}
.user-nav{
    display: flex;
    align-items: center;
    align-self: stretch;

    & > *{
        padding: 0 2rem;
        cursor: pointer;
        height: 100%;
        display: flex;
        align-items: center;

    }

    & > *:hover{
        background-color: var(--color-grey-light-3);
    }
   
    &__icon-box{
        display: flex;
        align-items: center;
        position: relative
    }
    &__icon{
        height: 2.6rem;
        width: 2.6rem;
        fill: #fff
     

    }
    &__bell{
        font-size: 1.2rem;
        height: 1.7rem;
        width: 1.7rem;
        border-radius:50%;   
        background-color: red;
        color: #fff;
        position: absolute;
        top: 1rem;
        right: 1.4rem;
        display: flex;
        justify-content: center;
        align-items: center;

     }

    &__user-photo{
        height: 3.75rem;
        border-radius: 50%;
        margin-right: 1rem;
        
    }
    
   
}
</style>
