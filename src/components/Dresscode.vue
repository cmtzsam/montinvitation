<template>
  <section class="Dresscode">
    <div class="o-container">

      <h2><span>Código de vestimenta</span></h2>

      <div class="Dresscode--main">
        <div class="fondo cherryblossom">
          <!-- <h5>Romantico Bohemio</h5> -->
          <img src="@/assets/images/dress1.png" colorcode="cherryblossom" class="img-full-responsive imgactive">
          <img src="@/assets/images/dress2.png" colorcode="orchidhush" class="img-full-responsive ">
          <img src="@/assets/images/dress3.png" colorcode="peachbud" class="img-full-responsive">
          <img src="@/assets/images/dress4.png" colorcode="lettucegreen" class="img-full-responsive">
        </div>
        <!-- <h3>Pantone </h3> -->
      </div>
      <div class="Dresscode--pantones">
        <div @click="cambiovestimenta" class="Dresscode--code cherryblossom codeactive" colorcode="cherryblossom">
          <div class="box"></div>
          <div class="Dresscode-info">
            <p>Pantone</p>
            <h3>13-3207</h3>
            <h4>Cherry Blossom</h4>
          </div>
        </div>
        <div @click="cambiovestimenta" class="Dresscode--code orchidhush" colorcode="orchidhush">
          <div class="box"></div>
          <div class="Dresscode-info">
            <p>Pantone</p>
            <h3>13-3805</h3>
            <h4>Orchid Hush</h4>
          </div>
        </div>
        <div @click="cambiovestimenta" class="Dresscode--code peachbud" colorcode="peachbud">
          <div class="box"></div>
          <div class="Dresscode-info">
            <p>Pantone</p>
            <h3>14-1324</h3>
            <h4>Peach Bud</h4>
          </div>
        </div>
        <div @click="cambiovestimenta" class="Dresscode--code lettucegreen" colorcode="lettucegreen">
          <div class="box"></div>
          <div class="Dresscode-info">
            <p>Pantone</p>
            <h3>13-0324</h3>
            <h4>Lettuce Green</h4>
          </div>
        </div>
      </div>

    </div>
  </section>
</template>
<script>

  export default{

    mounted(){
      this.cambiovestimenta = (e) => {
        let current_color = e.currentTarget.getAttribute('colorcode');
        let codes = document.querySelectorAll('.Dresscode--code');
        let fondo = document.querySelector('.Dresscode--main .fondo');
        let pictures = document.querySelectorAll('.Dresscode--main .fondo img');

        // fondo.classList.contains('fondoactive') && fondo.classList.remove('codeactive')
        fondo.removeAttribute('class')
        fondo.setAttribute('class', `fondo ${current_color}`)

        // Encender la imagen correspondiente
        Array.from(codes).forEach( code => {
          code.classList.contains('codeactive') && code.classList.remove('codeactive')
          if ( current_color == code.getAttribute('colorcode') ){
            code.classList.add('codeactive');
          }
        });        
        // Encender la imagen correspondiente
        Array.from(pictures).forEach( pic => {
          pic.classList.contains('imgactive') && pic.classList.remove('imgactive')
          if ( current_color == pic.getAttribute('colorcode') ){
            pic.classList.add('imgactive');
          }
        });
      };
    }

  }

</script>
<style lang="sass">
@import './Dresscode'
</style>