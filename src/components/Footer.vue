<template>
    <footer class="container-fluid">
        <div class="row">
            <footer class="lead">Nusaibah's Portfolio &copy; <span class="shadow">{{ cYear }} | 
                <a href="https://github.com/Nusaibah01" target="_blank"> <i class="bi bi-github"></i></a></span> | <a href="https://www.linkedin.com/in/nusaibah-abderemane-charif-351127308/" target="_blank"><i class="bi bi-linkedin"></i></a>
            </footer>
        </div>
    </footer>
</template>

<script>


export default {
name: 'FooterComp',
data() {
    return{
        cYear: new Date().getUTCFullYear()
    }
},

}
</script>

<style scoped>


</style>