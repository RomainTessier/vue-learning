<template>
  <div class="form">
  <form>
      <label>Email</label>
      <input type="email" v-model="email"/>

      <label>Password</label>
      <input type="password" v-model="password"/>
  </form>

  <label>Role:</label>
  <select v-model="role">
      <option value="admin">Admin</option>
      <option value="user">User</option>
  </select>

  <label>Accept terms and conditions</label>
  <input type="checkbox" v-model="terms" required>
  
<div class="input">
  <div>email : {{ email }}</div>
  <div>password : {{ password }}</div>
  <div>role : {{ role }}</div>
  <div>terms : {{ terms }}</div>
</div>
</div>
</template>


<script>
export default {
  name: 'SignupForm',
  data() {
      return {
          email: '',
          password: '',
          role: '',
          terms: false
      }
  }
}
</script>

<style>
.form, form {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 10vh;
  gap: 1vh;
}

.input{
  padding: 2vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1vh;
}
</style>
