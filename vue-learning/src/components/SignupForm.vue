<template>
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

    <input type="checkbox" v-model="terms" required>
    <label>Accept terms and conditions</label>

    <div>email : {{ email }}</div>
    <div>password : {{ password }}</div>
    <div>role : {{ role }}</div>
    <div>terms : {{ terms }}</div>
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

</style>