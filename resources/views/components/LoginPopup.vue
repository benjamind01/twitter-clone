<template>
    <div class="popup">
        <div class="popup-inner bg-black flex flex-col text-left justify-center items-center py-4  w-[600px] rounded-2xl">
            <div class="flex items-center justify-between flex-row w-full px-4">
                <div>
                    <button @click="() => TogglePopup()" class="text-white font-bold text-xl hover:bg-gray-800 px-2 py-1 rounded-full transition-all">X</button>
                </div>
                <svg viewBox="0 0 24 24" aria-hidden="true" class="w-[5%] fill-[#d6d9db]">
                        <g><path d="M23.643 4.937c-.835.37-1.732.62-2.675.733.962-.576 1.7-1.49 2.048-2.578-.9.534-1.897.922-2.958 1.13-.85-.904-2.06-1.47-3.4-1.47-2.572 0-4.658 2.086-4.658 4.66 0 .364.042.718.12 1.06-3.873-.195-7.304-2.05-9.602-4.868-.4.69-.63 1.49-.63 2.342 0 1.616.823 3.043 2.072 3.878-.764-.025-1.482-.234-2.11-.583v.06c0 2.257 1.605 4.14 3.737 4.568-.392.106-.803.162-1.227.162-.3 0-.593-.028-.877-.082.593 1.85 2.313 3.198 4.352 3.234-1.595 1.25-3.604 1.995-5.786 1.995-.376 0-.747-.022-1.112-.065 2.062 1.323 4.51 2.093 7.14 2.093 8.57 0 13.255-7.098 13.255-13.254 0-.2-.005-.402-.014-.602.91-.658 1.7-1.477 2.323-2.41z"></path></g>
                </svg>
                <div>
                    
                </div>
            </div>
            <div class="py-28">
            <h2 class="text-[#E7E9EA] font-extrabold text-[28px] text-left mt-8">Sign in to Twitter</h2>
            <form method="POST" action="#" class="flex flex-col">
                <input class="bg-black indent-2 border-gray-700  rounded-md border-[1px] py-4 w-[300px] mt-4" type="text" placeholder="Phone, email, or username">
                <input type="submit" value="Next" class="bg-gray-100 py-[6px] mt-8 rounded-full text-Chirp font-bold" />
            </form>
            <a href="#" class="mt-6 bg-none border-[1px] border-gray-600 text-sm text-white  w-[300px] py-[6px] rounded-full text-center font-bold flex flex-row justify-center items-center" ><button>Forgot Password?</button></a>
            <p class="text-[#71767b] text-md font-medium mt-14 text-left">Don't have an account ? <a href="#" class="text-[#1d9cf0] hover:border-b-[1px] border-[#1d9cf0] ">Sign Up</a></p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.popup {
	position: fixed;
	top: 0;
	left: 0;
	right: 0;
	bottom: 0;
	z-index: 99;
	background-color: rgba(91, 112, 131, 0.4);
	
	display: flex;
	align-items: center;
	justify-content: center;
}
</style>

<script setup lang="ts">

defineProps<{
    TogglePopup()
}>()

</script>