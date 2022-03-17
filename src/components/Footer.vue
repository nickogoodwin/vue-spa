<template>
    <footer class="text-center bg-dark text-light">
        <img id="vue-logo" src="../assets/logo.png">
        <p>Copyright &copy; {{getYear}}</p>
        <p>Page Created by {{author}}</p>
    </footer>
</template>

<script>
export default {
    name: 'sectionFooter',
    data: function() {
        return {
            author: 'Nicko Goodwin'
        }
        
    },
    computed: {
        getYear: function() {
            let now = new Date();
            return now.getFullYear();
        }
    },
}
</script>

<style>
    #vue-logo {
        width: 100px;
        height: 100px;
    }

    footer {
        padding: 1em;
    }
</style>