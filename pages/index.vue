<template>
    <div>
      
        <div class="content">
            <Sidebar/>

           <div class="video-content container mt-5">
               <div class="row">
                   <div class="col-12 col-lg-3">
                      <video-card/>
                   </div>
                   <div class="col-12 col-lg-3">
                      <video-card/>
                   </div>
                   <div class="col-12 col-lg-3">
                      <video-card/>
                   </div>
                   <div class="col-12 col-lg-3">
                      <video-card/>
                   </div>
                   <div class="col-12 col-lg-3">
                      <video-card/>
                   </div>
                   <div class="col-12 col-lg-3">
                      <video-card/>
                   </div>
                   <div class="col-12 col-lg-3">
                      <video-card/>
                   </div>
                
                
                   
                 
                </div>
               </div> 
        </div>
    </div>

</template>

<script>
export default {}
</script>

<style>
.content{
    display: flex;
    flex-direction: row;
}
.video-content{
    display: flex;
    flex-basis: 83%;
}
</style>
