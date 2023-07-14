<script setup>
let register = ref(false);
</script>
<template>
    <section class="bg-red-500 flex flex-col justify-center items-center">
        <div class="bg-red-300 p-4 rounded-lg my-96">
            <form method="post" v-if="register == false">
                <h1 class="font-semibold text-xl text-white text-center">
                    Login
                </h1>
                <label for="email" class="text-white text-lg">Email</label>
                <input
                    type="text"
                    name="email"
                    id="email"
                    class="block w-80 text-lg text-black py-1 px-5 rounded-lg border-2 mb-4 border-red-400 focus:outline-none focus:border-red-700"
                />
                <label for="password" class="text-white text-lg"
                    >Password</label
                >
                <input
                    type="password"
                    name="password"
                    id="password"
                    class="block w-80 text-lg text-black py-1 px-5 rounded-lg border-2 border-red-400 focus:outline-none focus:border-red-700 mb-11"
                />
                <input
                    type="submit"
                    value="Log In"
                    class="block w-80 bg-white text-black py-1 px-5 rounded-lg border-2 border-red-400 hover:bg-gray-100"
                />
            </form>
            <form method="post" v-else>
                <h1 class="font-semibold text-xl text-white text-center">
                    Register
                </h1>
                <label for="email" class="text-white text-lg">Email</label>
                <input
                    type="text"
                    name="email"
                    id="email"
                    class="block w-80 text-lg text-black py-1 px-5 rounded-lg border-2 mb-4 border-red-400 focus:outline-none focus:border-red-700"
                />
                <label for="password1" class="text-white text-lg"
                    >Password</label
                >
                <input
                    type="password"
                    name="password1"
                    id="password1"
                    class="block w-80 text-lg text-black py-1 px-5 rounded-lg border-2 border-red-400 focus:outline-none focus:border-red-700 mb-3"
                />
                <label for="password2" class="text-white text-lg"
                    >Confirm password</label
                >
                <input
                    type="password"
                    name="password2"
                    id="password2"
                    class="block w-80 text-lg text-black py-1 px-5 rounded-lg border-2 border-red-400 focus:outline-none focus:border-red-700 mb-10"
                />
                <input
                    type="submit"
                    :value="register ? 'Sign In' : 'Log In'"
                    class="block w-80 bg-white text-black py-1 px-5 rounded-lg border-2 border-red-400 hover:bg-gray-100"
                />
            </form>
            <p class="text-white mt-3" v-if="register">
                Already have an account?
                <span
                    class="underline cursor-pointer font-semibold"
                    v-on:click="register = !register"
                    >Log In</span
                >
            </p>
            <p class="text-white mt-3" v-else>
                Dont have an account?
                <span
                    class="underline cursor-pointer font-semibold"
                    v-on:click="register = !register"
                    >Register</span
                >
            </p>
        </div>
    </section>
</template>
