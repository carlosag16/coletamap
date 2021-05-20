<template>
    <div>
        <!-- <h1>Locais de descarte</h1> -->
        <p> {{coordinates.lat}} latitude, {{coordinates.lng}} londitude </p>
    </div>
</template>

<script>
export default {
    data() {
        return{
            coordinates: {
                lat: 0,
                lng: 0
            }
        }
    },
    created(){
        this.$getLocation({})
            .then(coordinates => {
                this.coordinates = coordinates;

            })
            .catch(error => alert(error));
    }
}
</script>
