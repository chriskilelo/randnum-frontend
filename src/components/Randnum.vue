<template>
    <div class="p-10">
        <div>
            <label
                class="flex justify-center mb-9 text-4xl whitespace-nowrap font-medium text-gray-700 md:w-1/2 md:justify-start">
                Random Numbers
            </label>
            <input type="text" name="random_number" id="random_number"
                class="flex mb-4 w-full bg-slate-100 border border-gray-300 rounded-lg p-4 focus:outline-gray-300 text-2xl lg:w-3/4 xl:w-1/2">
        </div>
        <div>
            <button type="button"
                class="mr-1 w-full p-4 rounded-lg bg-blue-500 text-white font-medium text-2xl md:w-1/2 lg:w-1/3 xl:w-1/5"
                @click="giveGlory()"> Generate
            </button>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            mx: '50',
            my: '50'
        }
    },
    methods: {
        giveGlory() {
            alert('JESUS IS LORD AND KING' + '\n' + this.mx + this.my)
        },
        updateMethod(){

        },
        async function getUser() {
  try {
    const response = await axios.get('/user?ID=12345');
    console.log(response);
  } catch (error) {
    console.error(error);
  }
}
    }
}
</script>