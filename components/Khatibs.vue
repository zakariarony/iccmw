<template>
    <section class="container">
        <h2 class="text-center py-4">This Month Jummah Khatib's</h2>
        <div class="row justify-content-around">
            <div class="col-md-3 pb-3 pb-md-0" v-for="khatib in khatibs">
                <div class="card">
                    <img :src="khatib.img" class="card-img-top khatibImg" alt="...">
                    <div class="card-body text-center">
                        <h5 class="card-title">{{khatib.name}}</h5>
                    </div>
                </div>
            </div>
        </div>
        <h3 class="text-center py-4 mt-5">Please subscribe to get Mosque related event notifications</h3>
        <div class="row px-3 py-3  py-lg-5 px-lg-5 subscribePart">
            <div class="col-lg-5 col-md-5 col-sm-6 col-xs-12">
                <input
                        class="subscribe__form-text"
                        type="email"
                        placeholder="YOUR EMAIL"
                >
            </div>
            <div class="col-lg-5 col-md-4 col-sm-6 col-xs-12 pt-3 pt-sm-0">
                <input
                        class="subscribe__form-text"
                        type="number"
                        placeholder="YOUR PHONE">
            </div>
            <div class="col-lg-2 col-md-3 col-sm-12 col-xs-12 pt-3 pt-md-0">
                <input
                        class="subscribe__submit-btn w-100"
                        type="submit"
                        value="SUBSCRIBE"
                >
            </div>
        </div>
    </section>
</template>

<script>
    import MawlanaPic1 from '@/assets/images/mawlana1.jpg' ;
    import MawlanaPic2 from '@/assets/images/mawlana2.jpg' ;
    import MawlanaPic3 from '@/assets/images/mawlana3.png' ;
    import MawlanaPic4 from '@/assets/images/mawlana4.jpg' ;
    export default {
        name: "Khatibs",
        data(){
            return {
                khatibs: [
                    {
                        name: 'Abdul Jalal',
                        img: MawlanaPic1
                    },
                    {
                        name: 'Abdul Karim',
                        img: MawlanaPic2
                    },
                    {
                        name: 'Abdul Based',
                        img: MawlanaPic3
                    },
                    {
                        name: 'Abdul Awal',
                        img: MawlanaPic4
                    }
                ]
            }
        }
    }
</script>

<style scoped>
    .subscribe__form-text {
        padding: 10px 20px 10px 20px;
        font-weight: 600;
        width: 100%;
    }
    .subscribe__submit-btn{
        padding: 12px;
        background-color: #291f1f;
        color: white;
        border: none;
        font-weight: 600;
    }
    .subscribePart{
        background-color: green;
    }
    .khatibImg{
        height: 210px !important;
    }
</style>