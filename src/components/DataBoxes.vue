<template>
    <div class="grid md:grid-cols-2 gap-4">
        <!--    BOX 1  -->
        <div class="shadow-md bg-purple-200 p-10 text-center">
            <h3 class="text-3xl text-purple-900 font-bold mb-4">Cases</h3>
        <div class="text-2xl">
            <span class="font-bold">New:</span>
            {{numberWithCommas(stats.NewConfirmed)}}
        </div>
        <div class="text-2xl">
            <span class="font-bold">Total:</span>
            {{numberWithCommas(stats.TotalConfirmed)}}
        </div>
        
        </div>
         <!--   BOX 2  -->
        <div class="shadow-md bg-purple-300 p-10 text-center">
            <h3 class="text-3xl text-purple-900 font-bold mb-4">Deaths</h3>
        <div class="text-2xl">
            <span class="font-bold">New:</span>
            {{numberWithCommas(stats.NewDeaths)}}
        </div>
        <div class="text-2xl">
            <span class="font-bold">Total:</span>
            {{numberWithCommas(stats.TotalDeaths)}}
        </div>
        
        </div>



    </div>

</template>

<script>
export default {
    name:'DataBoxes',
    props:['stats'],
    setup() {
        return{
            numberWithCommas(x) {
            return x.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ',');
        }

        };
        
    }
};
</script>