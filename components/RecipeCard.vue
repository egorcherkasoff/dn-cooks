<template>
    <article
        class="bg-red-400 flex p-4 rounded-lg text-white justify-between items-center h-48"
    >
        <img
            src="https://static.wikia.nocookie.net/aa5f6557-a572-49c0-8ce7-57d6d7869154/scale-to-width/755"
            alt="Recipe image"
            height="200px"
            width="200px"
            class="object-cover w-40 h-40 rounded-lg"
        />
        <div class="block ms-5 text-lg">
            <NuxtLink
                to="/"
                class="font-semibold border-b-2 border-red-400 transition-all ease-out hover:border-white"
                >Berried Delight</NuxtLink
            >
            <p><span class="font-semibold">Category: </span>Dessert</p>
            <p>
                <span class="font-semibold overflow-hidden">About: </span>Lorem
                ipsum dolor sit amet, consectetur adipisicing elit. Quos
                accusantium velit consectetur facilis culpa ex reprehenderit a
                maiores temporibus voluptatum expedita aliquid earum deserunt...
            </p>
        </div>
        <div class="ms-5 text-lg flex flex-col items-center w-32">
            <Icon
                name="material-symbols:bookmark-outline-rounded"
                class="text-5xl text-gray-50 text-center cursor-pointer hover:text-yellow-500"
            ></Icon>
            <p class="block text-center font-semibold">
                <span>Rating: </span>5 / 5
            </p>
            <!-- bookmark заполненная -->
        </div>
    </article>
</template>

<script>
export default {};
</script>
