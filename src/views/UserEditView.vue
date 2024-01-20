<template>
    <div>
        <pre>
            {{ $route.params }}
        </pre>
        Usuário <br>
        <button @click="login()">
            Login
        </button>
    </div>
</template>

<script>
export default {
    created() {
        console.log(this.$router);
    },
    methods: {
        login() {
            this.$router.push('/')
            console.log('logado');
        }
    }
}
</script>