<template>
    <div class="pt-16">
        <h1 class="text-3xl font-semibold mb-4">Where are we going?</h1>
        <form action="#">
            <div class="overflow-hidden shadow sm:rounded-md max-w-sm mx-auto text-left">
                <div class="bg-white px-4 py-5 sm:p-6">
                    <div>
                        <GMapAutocomplete 
                         placeholder="My destination"
                         @place_changed = "handleLocationChanged"
                         class="mt-1 block w-full px-3 py-3 rounded-md border border-gray-300 shadow-sm">
                        </GMapAutocomplete>

                    </div>


                </div>
                <div class="bg-gray-50 px-4 py-5 text-right sm:p-6">
                    <div>
                        <button type="text" 
                        class=" text-white p-2 inline-flex justify-center rounded-md border border-transperent bg-black py2">
                        Find a ride</button>
                    </div>
                </div>

            </div>
        </form>
    </div>
</template>

<script setup> 
    const handleLocationChanged = (e) => {
        console.log('handleLocationChanged', e)
    }   
</script>