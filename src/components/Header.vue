<script>
export default {
  name: 'Header'

}
</script>

<template>
  <header>
      <div class="container ">
          
            <ul class="menu">
              <li><a href="#">Donna</a></li>
              <li><a href="#">Uomo</a></li>
              <li><a href="#">Bambini</a></li>
            </ul>
          
          
            <img class="logo" src="/boolean-logo.png" alt="logo" />
          
            <ul class="menu">
              <li>
                <a href=""><i class="fa-regular fa-user"></i></a>
              </li>
              <li>
                <a><i class="fa-regular fa-heart"></i></a>
              </li>
              <li>
                <a href=""><i class="fa-solid fa-bag-shopping"></i></a>
              </li>
            </ul>
          
      </div>
    </header>
</template>


<style lang="scss" scoped>
  @use '../scss/partials/General.scss' as *;
  @use '../scss/partials/typography.scss' as *;
  @use '../scss/partials/variabiles.scss' as *;
  header{
    background-color: $header-bg;
    height: 80px;
    display: flex;
    align-items: center;
    z-index: 999;
    position: fixed;
    top:0;
    width: 100%;

    .container{
      display: flex;
      justify-content: space-between;
      align-items: center;
      

       .logo{
          width: 200px; 
          display: flex; 
          align-self: center;
        } 

        li{
          display: inline;
          margin: 7px;
        }
    }
    

    
  }


  
</style>