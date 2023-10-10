<script>
export default {
  name: "Main",
};
</script>

<template>
    <main>
        <div class="container-main container">
            <div class="product">
                <div class="switch">
                    <img  class="modello uno" src="../assets/img/1.webp" alt="">
                    <img  class="modello due" src="../assets/img/1b.webp" alt="">
                </div>
               <div class="lable">
                    <span class="discount">-50%</span>
                    <span class="green">Sostenibilità</span>
               </div>
               <span class="hearts">&hearts;</span>
                <span>Come Zucchero Filato</span>
                <h2>VOGLIA DI COLORI PASTELLO</h2>
                <span class="euro-red">129,99 &euro;</span> <span class="euro-bar">184,99 &euro;</span>
            </div>

            <div class="product">
                <div class="switch">
                    <img  class="modello uno" src="../assets/img/2.webp" alt="">
                    <img  class="modello due" src="../assets/img/2b.webp" alt="">
                </div>
               <div class="lable">
                    <span class="discount">-50%</span>
                    <span class="green">Sostenibilità</span>
               </div>
               <span class="hearts">&hearts;</span>
                <span>Come Zucchero Filato</span>
                <h2>VOGLIA DI COLORI PASTELLO</h2>
                <span class="euro-red">129,99 &euro;</span> <span class="euro-bar">184,99 &euro;</span>
            </div>

            <div class="product">
                <div class="switch">
                    <img  class="modello uno" src="../assets/img/3.webp" alt="">
                    <img  class="modello due" src="../assets/img/3b.webp" alt="">
                </div>
               <div class="lable">
                    <span class="discount">-50%</span>
                    <span class="green">Sostenibilità</span>
               </div>
               <span class="hearts">&hearts;</span>
                <span>Come Zucchero Filato</span>
                <h2>VOGLIA DI COLORI PASTELLO</h2>
                <span class="euro-red">129,99 &euro;</span> <span class="euro-bar">184,99 &euro;</span>
            </div>

            <div class="product">
                <div class="switch">
                    <img  class="modello uno" src="../assets/img/4.webp" alt="">
                    <img  class="modello due" src="../assets/img/4b.webp" alt="">
                </div>
               <div class="lable">
                    <span class="discount">-50%</span>
                    <span class="green">Sostenibilità</span>
               </div>
               <span class="hearts">&hearts;</span>
                <span>Come Zucchero Filato</span>
                <h2>VOGLIA DI COLORI PASTELLO</h2>
                <span class="euro-red">129,99 &euro;</span> <span class="euro-bar">184,99 &euro;</span>
            </div>

            <div class="product">
                <div class="switch">
                    <img  class="modello uno" src="../assets/img/5.webp" alt="">
                    <img  class="modello due" src="../assets/img/5b.webp" alt="">
                </div>
               <div class="lable">
                    <span class="discount">-50%</span>
                    <span class="green">Sostenibilità</span>
               </div>
               <span class="hearts">&hearts;</span>
                <span>Come Zucchero Filato</span>
                <h2>VOGLIA DI COLORI PASTELLO</h2>
                <span class="euro-red">129,99 &euro;</span> <span class="euro-bar">184,99 &euro;</span>
            </div>

            <div class="product">
                <div class="switch">
                    <img  class="modello uno" src="../assets/img/6.webp" alt="">
                    <img  class="modello due" src="../assets/img/6b.webp" alt="">
                </div>
               <div class="lable">
                    <span class="discount">-50%</span>
                    <span class="green">Sostenibilità</span>
               </div>
               <span class="hearts">&hearts;</span>
                <span>Come Zucchero Filato</span>
                <h2>VOGLIA DI COLORI PASTELLO</h2>
                <span class="euro-red">129,99 &euro;</span> <span class="euro-bar">184,99 &euro;</span>
            </div>
          </div>
      
  </main>
</template>


<style lang="scss" scoped>
  @use '../scss/partials/General.scss' as *;
  @use '../scss/partials/typography.scss' as *;
  @use '../scss/partials/variabiles.scss' as *;

 
    .container-main{
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        margin-top: 100px;
        margin-bottom: 50px;

        .product{
            position: relative;
            width:calc(100% / 3.1);
            margin-bottom: 50px;
            

            .modello{
                width: 100%;
                height: auto;
                cursor: pointer;
            }

            .switch:hover .modello.uno{
                display: none;

            }

            .switch:hover .modello.due{
                display: block;
            }

            .modello.uno {
                 display: block;
            }
            .modello.due{
                display:none ;
            }

            .lable{
                position: absolute;
                bottom: 120px;
                left:0px;
                color: white;
                font-size: 0,8rem;

                .discount{
                    background-color: red;
                    padding: 3px 3px;
                }
                .green{
                    background-color: green;
                    padding: 3px 5px;
                }

                
            }

            .hearts{
                position: absolute;
                top:10px;
                right: 0px;
                padding: 5px 5px;
                background-color: white;

            }

            .euro-red{
                color: red;
            }

            .euro-bar{
                text-decoration: line-through;
            }
        }
    
    }     
</style>