<template>
    <div class="hero-body">
        <div class="container has-text-centered">
        <div class="column is-6 is-offset-3">
          <h1 class="title">
            Сайт у розробці
          </h1>
          <h2 class="subtitle">
            Комп'ютеризовані системи та програмування <br>
            Гурток для обдарованої молоді Шостки
          </h2>
          <div class="box">
            
            <div class="field is-grouped">
              <p class="control is-expanded">
                <input class="input" type="text" placeholder="Введіть свій email">
              </p>
              <p class="control">
                <a class="button is-dark" @click="mailSend">
                  Повідом Мене
                </a>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>


<script>
  export default {
    methods: {
      mailSend () {
        // console.log('send maill button')
      }
    }
  }
</script>