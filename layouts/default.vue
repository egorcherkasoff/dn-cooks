<template>
    <header class="py-5 bg-red-400 text-white">
        <nav class="flex justify-between container mx-auto items-center">
            <NuxtLink to="/" class="text-xl font-bold">DN Cooks</NuxtLink>
            <ul class="flex text-lg font-semibold">
                <li>
                    <NuxtLink
                        to="/"
                        class="border-b-2 border-red-400 transition-all ease-out hover:border-white"
                        >Recipes</NuxtLink
                    >
                </li>
                <li>
                    <NuxtLink
                        to="/"
                        class="ms-10 border-b-2 border-red-400 transition-all ease-out hover:border-white"
                        >Login</NuxtLink
                    >
                </li>
            </ul>
        </nav>
    </header>
    <main>
        <slot></slot>
    </main>

    <footer class="py-5 bg-red-700 text-white">
        <nav class="container mx-auto flex justify-between items-center">
            <div>
                <NuxtLink to="/" class="text-xl font-bold">DN Cooks</NuxtLink>
                <p class="text-xs">
                    by
                    <a href="https://github.com/egorcherkasoff" target="_blank"
                        >@egorcherkasoff</a
                    >
                </p>
            </div>
            <ul class="flex text-lg font-semibold">
                <li>
                    <NuxtLink
                        to="/"
                        class="border-b-2 border-red-700 transition-all ease-out hover:border-white"
                        >Recipes</NuxtLink
                    >
                </li>
                <li>
                    <NuxtLink
                        to="/"
                        class="ms-10 border-b-2 border-red-700 transition-all ease-out hover:border-white"
                        >Login</NuxtLink
                    >
                </li>
            </ul>
        </nav>
    </footer>
</template>

<script></script>
