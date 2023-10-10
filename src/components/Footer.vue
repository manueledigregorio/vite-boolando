<script>
export default {
  name: 'Footer'
}
</script>

<template>
  <footer>
        <div class="container  ">

            <div>
                <h3>Booleando S.r.l.</h3>
                <span>Informazioni legali</span>
                <span>informativa sulla privacy</span>
                <span>Diritto di recesso</span>
            </div>
            <div>
                <span>Trovaci anche su</span>
                <ul>
                    <li><a><i class="fa-brands fa-twitter"></i></a></li>
                    <li><a><i class="fa-brands fa-square-facebook"></i>
                    </a></li>
                    <li><a><i class="fa-brands fa-instagram"></i></a></li>
                    <li><a><i class="fa-brands fa-pinterest"></i></a></li>
                    <li><a><i class="fa-brands fa-youtube"></i></a></li>
                </ul>
            </div>
        </div>
    </footer>
</template>


<style lang="scss" scoped>
 @use '../scss/partials/General.scss' as *;
  @use '../scss/partials/typography.scss' as *;
  @use '../scss/partials/variabiles.scss' as *;

  footer{
    background-color:$black ;
    padding-top:40px ;
    padding-bottom: 30px;
    color: $white;

    .container{
      display: flex;
      justify-content: space-between;
      align-items: start;
    }
    ul{
      display: flex;
    }

    li{
      margin: 7px;
    }
   
  }
</style>