<script setup lang="ts">
// Cansei, mas falta terminar aqui o nav bar

</script>

<template>
    <nav class="flex items-center justify-between px-16 py-6">
        <div>
            <img 
                src="/public/icon/logo.svg" 
                alt="Logo do Teammates"
                class="w-8"
                >
        </div>

        <div class="flex flex-row items-center justify-start">
            <a href="#inicio"  
               class="text-[var(--text-nav-color)]">Início
            </a>

            <a href="#projetos"  
               class="text-[var(--text-nav-color)]">Projetos
            </a>

            <a href="#equipe"  
               class="text-[var(--text-nav-color)]">Equipe
            </a>

            <a href="#faculdade"  
               class="text-[var(--text-nav-color)]">Faculdade
            </a>

        </div>
    </nav>
</template>

<style scoped>

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

</style>