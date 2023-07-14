<template>
    <section class="text-center bg-red-400 py-28 text-white">
        <h1 class="text-4xl font-bold tracking-wider">DN Cooks</h1>
        <p class="text-lg tracking-wide font-semibold mb-4">
            For all your cooking needs
        </p>
        <NuxtLink
            to="/"
            class="tracking-widest border-b-2 border-red-400 transition-all ease-out hover:border-white"
            >discover recipes</NuxtLink
        >
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
    <div class="bg-red-500 py-5">
        <section class="container mx-auto text-white">
            <h1 class="text-center font-semibold text-xl">
                Discover recipes from around the world
            </h1>
        </section>
        <section class="container mx-auto text-white">
            <h2 class="text-xl mb-2 mt-1 ps-1">Popular recipes</h2>
            <div class="grid gap-5 grid-cols-2 grid-rows-2">
                <RecipeCard></RecipeCard>
                <RecipeCard></RecipeCard>
                <RecipeCard></RecipeCard>
                <RecipeCard></RecipeCard>
            </div>
        </section>
        <section class="container mx-auto text-white">
            <h2 class="text-xl mb-2 mt-1 ps-1">New recipes</h2>
            <div class="grid gap-5 grid-cols-2 grid-rows-2">
                <RecipeCard></RecipeCard>
                <RecipeCard></RecipeCard>
                <RecipeCard></RecipeCard>
                <RecipeCard></RecipeCard>
            </div>
        </section>
        <section class="container mx-auto text-white">
            <h2 class="text-xl mb-2 mt-1 ps-1">Categories</h2>
            <Swiper
                :modules="[SwiperPagination]"
                :space-between="50"
                :slides-per-view="6"
                :pagination="{ clickable: true }"
                :breakpoints="{
                    0: { slidesPerView: 1, spaceBetween: 0 },
                    576: { slidesPerView: 2, spaceBetween: 0 },
                    768: { slidesPerView: 3, spaceBetween: 0 },
                    1024: { slidesPerView: 4, spaceBetween: 0 },
                    1280: { slidesPerView: 5, spaceBetween: 0 },
                    1530: { slidesPerView: 6, spaceBetween: 50 },
                }"
            >
                <SwiperSlide><CategoryCard></CategoryCard></SwiperSlide>
                <SwiperSlide><CategoryCard></CategoryCard></SwiperSlide>
                <SwiperSlide><CategoryCard></CategoryCard></SwiperSlide>
                <SwiperSlide><CategoryCard></CategoryCard></SwiperSlide>
                <SwiperSlide><CategoryCard></CategoryCard></SwiperSlide>
                <SwiperSlide><CategoryCard></CategoryCard></SwiperSlide>
                <SwiperSlide><CategoryCard></CategoryCard></SwiperSlide>
                <SwiperSlide><CategoryCard></CategoryCard></SwiperSlide>
                <SwiperSlide><CategoryCard></CategoryCard></SwiperSlide>
                <SwiperSlide><CategoryCard></CategoryCard></SwiperSlide>
            </Swiper>
        </section>
    </div>
</template>
