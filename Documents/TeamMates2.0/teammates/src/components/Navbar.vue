<script setup lang="ts">
import { ref } from 'vue'

const activeItem = ref('inicio')

const setActive = (item: string) => {
    activeItem.value = item
}
</script>

<template>
    <div class="fixed top-0 left-0 z-50 flex w-full items-center justify-center gap-2 py-6">

        <!-- Logo -->
        <div class="flex h-14 w-14 items-center justify-center rounded-full border border-[#333] bg-[var(--background-color-glass)]">
            <img
                src="/icon/logo.svg"
                alt="Logo do Teammates"
                class="w-8"
            >
        </div>

        <!-- Navbar -->
        <nav class="flex items-center rounded-full border border-[#333] bg-[var(--background-color-glass)] px-6">

            <a
                href="#inicio"
                @click="setActive('inicio')"
                :class="activeItem === 'inicio'
                    ? 'text-[var(--detail-color)]'
                    : 'text-[var(--text-nav-color)] hover:text-[var(--detail-color)]'"
                class="relative flex h-14 w-28 items-center justify-center transition-colors"
            >
                Início

                <span
                    v-if="activeItem === 'inicio'"
                    class="absolute bottom-0 left-1/2 h-[2px] w-20 -translate-x-1/2 bg-[var(--detail-color)]"
                ></span>
            </a>

            <a
                href="#projetos"
                @click="setActive('projetos')"
                :class="activeItem === 'projetos'
                    ? 'text-[var(--detail-color)]'
                    : 'text-[var(--text-nav-color)] hover:text-[var(--detail-color)]'"
                class="relative flex h-14 w-28 items-center justify-center transition-colors"
            >
                Projetos

                <span
                    v-if="activeItem === 'projetos'"
                    class="absolute bottom-0 left-1/2 h-[2px] w-20 -translate-x-1/2 bg-[var(--detail-color)]"
                ></span>
            </a>

            <a
                href="#equipe"
                @click="setActive('equipe')"
                :class="activeItem === 'equipe'
                    ? 'text-[var(--detail-color)]'
                    : 'text-[var(--text-nav-color)] hover:text-[var(--detail-color)]'"
                class="relative flex h-14 w-28 items-center justify-center transition-colors"
            >
                Equipe

                <span
                    v-if="activeItem === 'equipe'"
                    class="absolute bottom-0 left-1/2 h-[2px] w-20 -translate-x-1/2 bg-[var(--detail-color)]"
                ></span>
            </a>

            <a
                href="#faculdade"
                @click="setActive('faculdade')"
                :class="activeItem === 'faculdade'
                    ? 'text-[var(--detail-color)]'
                    : 'text-[var(--text-nav-color)] hover:text-[var(--detail-color)]'"
                class="relative flex h-14 w-28 items-center justify-center transition-colors"
            >
                Faculdade

                <span
                    v-if="activeItem === 'faculdade'"
                    class="absolute bottom-0 left-1/2 h-[2px] w-20 -translate-x-1/2 bg-[var(--detail-color)]"
                ></span>
            </a>

        </nav>

    </div>
</template>
<style scoped>

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

</style>