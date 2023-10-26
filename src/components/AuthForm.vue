<template>
  <div>
    <h2>Форма регистрации</h2>
    <form @submit.prevent="register">
      <div>
        <label for="firstname">Имя:</label>
        <input type="text" id="firstname" v-model="user.firstname" required>
      </div>
      <div>
        <label for="lastname">Фамилия:</label>
        <input type="text" id="lastname" v-model="user.lastname" required>
      </div>
      <div>
        <label for="email">Email:</label>
        <input type="email" id="email" v-model="user.email" required>
      </div>
      <div>
        <label for="password">Пароль:</label>
        <input type="password" id="password" v-model="user.password" required>
      </div>
      <div>
        <label for="role">Роль:</label>
        <select id="role" v-model="user.role">
          <option value="ADMIN">Администратор</option>
          <option value="USER">Пользователь</option>
        </select>
      </div>
      <button type="submit">Зарегистрироваться</button>
    </form>
  </div>
</template>

<script>
import Component from "vue-class-component";
import Vue from "vue";

import axios from 'axios';
@Component
export default class AuthForm extends Vue {

  user = {
    firstname: '',
    lastname: '',
    email: '',
    password: '',
    role: 'USER', // Значение по умолчанию
  };

  register() {
    // Отправляем данные на сервер (замените URL на ваш реальный API)
    axios.post('https://api.example.com/register', this.user)
        .then(response => {
          console.log('Регистрация успешна', response.data);
        })
        .catch(error => {
          console.error('Произошла ошибка при регистрации', error);
        });
  }

}
</script>
