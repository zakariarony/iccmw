<template>
    <section class="container">
        <h2 class="text-center py-4">This Month Jummah Khatib's</h2>
        <div class="row justify-content-around">
            <div class="col-md-3 pb-3 pb-md-0" v-for="n in 4">
                <div class="embed-responsive embed-responsive-16by9">
                    <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/zpOULjyy-n8?rel=0" allowfullscreen></iframe>
                </div>
            </div>
        </div>
        <h3 class="text-center py-4 mt-5">Please subscribe to get Mosque related event notifications</h3>
        <div class="row px-3 py-3  py-lg-5 px-lg-5 subscribePart">
            <div class="col-lg-5 col-md-5 col-sm-6 col-xs-12">
                <!--
                <input
                        type="email"
                        class="form-control"
                        id="inputEmail"
                        placeholder="Email"
                >-->
                <input
                        class="subscribe__form-text"
                        type="email"
                        placeholder="YOUR EMAIL"
                >
            </div>
            <div class="col-lg-5 col-md-4 col-sm-6 col-xs-12 pt-3 pt-sm-0">
                <!--
                <input
                        type="number"
                        class="form-control"
                        id="inputPhone"
                        placeholder="Phone"
                >-->
                <input
                        class="subscribe__form-text"
                        type="number"
                        placeholder="YOUR PHONE">
            </div>
            <div class="col-lg-2 col-md-3 col-sm-12 col-xs-12 pt-3 pt-md-0">
                <!--
                <button type="submit" class="btn btn-primary mb-2 text-uppercase w-100">Subscribe</button>-->
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
    export default {
        name: "Khatibs"
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
</style>