<template>
  <q-page class="fit">
    <div class="row box">
      <div class="wd-img row justify-end">
        <q-img src="../assets/phone.png" class="phone"></q-img>
      </div>
      <div class="wd-log card "> 
        <q-card flat bordered class="my-card column  ">
          <q-card-section class="column items-center q-mt-sm">
            <q-img src="../assets/nome-instagram.png" class="name-insta"></q-img>
          </q-card-section>

          <q-card-section class="q-pt-md column items-center">
            <q-input outlined v-model="login" label="Número de celular, nome de usuário ou e-mail" class="put" ></q-input>
            <q-input outlined v-model="password" label="Senha" class="q-pt-xs put items-center" />
            <q-btn  color="primary" size="md" label="Iniciar sessão" class="put q-mt-sm"/>
          </q-card-section>

          <q-card-section class="row items-center justify-center" >
            <div class="line-bot q-mx-md"></div>
            <span class="or">OU</span>
            <div class="line-bot q-mx-md"></div>

          </q-card-section>
          <q-card-section class="column items-center">
            <span class="q-mb-sm"> <a href="" class="link text-weight-medium"> <q-icon size="2em" name="facebook" /> Iniciar sessão com Facebook </a></span>
            <span class="q-my-sm"><a href="" class="link text-caption q-mt-md">Esqueceu a senha?</a></span>
          </q-card-section>
        </q-card>
        <q-card flat bordered class="my-card column q-mt-sm">
          <q-card-section class="column items-center q-my-sm">
          <span>Não tem uma conta?<a href="" class="register"> Registrar-se</a></span>
          </q-card-section>
        </q-card>
        <div class="column items-center">
          <div class="q-ma-md">Obter aplicativo.</div>
          <div class="row">
          <q-img  src="../assets/apple-store.png" class="download q-mx-md"></q-img>
          <q-img  src="../assets/google-play.png" class="download q-mx-md"></q-img>
          </div>
        </div>
        </div>
        </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data() {
    return {
      login: '',
      password: '',
    }
  }
}
</script>

<style lang="scss">
  .wd-img  {
    width: 50%;
  }

  .wd-log {
    width: 50%;
  }

  .box {
    margin-top: 100px;
  }

  .phone {
    width: 500px;
  }

  .card {
    width: 400px;
    margin-top: 30px;
  }

  .name-insta {
    width: 200px;
  }

  .put {
    width: 300px;
  }

  .line-bot{
    width: 130px;
    border-bottom: 1px solid rgb(221, 221, 221);
  }

  .link {
    color: #3b5998;
    text-decoration: none;
  }

  .or {
    color: $grey-6;
    margin-top: -5px;
    font-weight: bold;
  }

  .register {
    color: #5f80c9;
    text-decoration: none;
    font-weight: bold;
  }

  .download{
    width: 140px;
    border-radius: 5px;
  }
</style>