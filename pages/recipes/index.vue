<template>
    <section class="text-center bg-red-400 py-24 text-white">
        <h1 class="text-4xl font-bold tracking-wider">Recipes</h1>
        <form method="get" class="flex justify-center mt-5">
            <input
                class="block w-80 text-lg text-black py-1 px-5 rounded-l-lg border-y-2 border-s-2 border-red-400 focus:outline-none focus:border-red-700"
                type="search"
                name="search"
            />
            <button
                type="submit"
                class="bg-white text-black border-red-400 rounded-r-lg border-red border-y-2 border-e-2 px-2 border-s-2 border-l-gray-200 hover:bg-gray-100"
            >
                Search
            </button>
        </form>
    </section>
    <div class="bg-red-500">
        <section class="container mx-auto"></section>
    </div>
</template>
