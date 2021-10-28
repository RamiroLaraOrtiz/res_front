<template>
  <div class="home">
    <div class="center">
      <div class="wrapper">
        <div class="space-in-components">
          <label for="email" class="distance-email-label ">Email</label>
          <input id="email" type="text" class="shadow-inputs padding-inputs">
        </div>
        <div class="space-in-components">
          <label for="password" class="pwd-distance ">Password</label>
          <input id="password" type="text" class="shadow-inputs padding-inputs">
        </div >
        <div class="center-btn-login space-in-components">
          <button class="shadow-btn size-btn-enter btn-style">ENTER</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
  }
}
</script>

<style scoped>
  .home{
    opacity:0.8;
    background: rgb(74,143,143);
    background: linear-gradient(47deg, rgba(74,143,143,1) 18%, rgba(72,142,142,1) 34%, rgba(59,129,129,1) 51%, rgba(70,143,143,1) 67%, rgba(69,167,167,1) 82%, rgba(46,165,189,0.8974974025933506) 100%);
    position:fixed;
    width:100%;
    height:100%;
    top:0px;
    left:0px;
    z-index:1000;
  }

  .wrapper {
    display: grid;
  }

  .center { 
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 100vh;
    align-items: center;
    justify-items: center;
  }

  .distance-email-label{
    margin-left: 30px;
    padding-right: 35px;
  }

  .pwd-distance{
    padding-right: 35px;
  }

  @font-face {
    font-family: 'TGL_31034-2';
    src: url('../assets/fonts/TGL_31034-2.ttf'),
  }

  .labels-login{ /* queda pendiente el que jale el tipo de font*/
    font-family: 'TGL_31034-2';
    color: white;
  }

  .center-btn-login{ 
    margin-left: 104px;
  }

  .space-in-components{
    margin-top: 31px;
  }

  .shadow-inputs{
    -webkit-box-shadow: -6px 6px 11px 6px rgba(0,0,0,0.8); 
    box-shadow: -6px 6px 11px 6px rgba(0,0,0,0.8);
    border: 2.5px solid #254d4d;
  }
   .shadow-btn{
    -webkit-box-shadow: -6px 6px 11px 6px rgba(0,0,0,0.8); 
    box-shadow: -6px 6px 11px 6px rgba(0,0,0,0.8);
    border: 2.5px solid #0d1b1b;
    border-radius: 8%;
  }

  .padding-inputs{
    padding-right: 68px;
  }
  .size-btn-enter{
    padding: 1px 23px 1px 23px;
  }

  .btn-style{
    color: #254d4d;
    background-color: #4fb4ad;
  }

</style>