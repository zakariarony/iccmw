<template>
    <div class="container py-5">
        <div class="row justify-content-around">
            <div class="col-xl-5 col-lg-5 col-md-6 col-sm-12">
                <h4 class="text-center pb-3">PRAYER TIMES</h4>
                <div class="prayerTime">
                    <div class="text-center py-2 prayerTimeCount">
                        <span>
                            Fajr In...
                        </span>
                        <h4>04:05:40</h4>
                    </div>
                    <table class="table table-striped table-dark">
                        <thead>
                        <tr>
                            <th scope="col">Salah</th>
                            <th scope="col">Adhan</th>
                            <th scope="col">Iqamah</th>
                        </tr>
                        </thead>
                        <tbody>
                        <tr>
                            <td>Fajr</td>
                            <td>06:13 AM</td>
                            <td>06:30 AM</td>
                        </tr>
                        <tr>
                            <td>Sunrise</td>
                            <td colspan="2">O7:20 AM</td>
                        </tr>
                        <tr>
                            <td>Duhur</td>
                            <td>01:00 PM</td>
                            <td>01:30 PM</td>
                        </tr>
                        <tr>
                            <td>Duhur</td>
                            <td>01:00 PM</td>
                            <td>01:30 PM</td>
                        </tr>
                        <tr>
                            <td>Magrib</td>
                            <td>01:00 PM</td>
                            <td>01:30 PM</td>
                        </tr>
                        <tr>
                            <td>Isha</td>
                            <td>01:00 PM</td>
                            <td>01:30 PM</td>
                        </tr>
                        <tr>
                            <td>Jummah</td>
                            <td>01:45 PM</td>
                            <td>02:15 PM</td>
                        </tr>
                        <tr>
                            <td>Khateeb</td>
                            <td colspan="2">Sh. Omar Ali</td>
                        </tr>
                        <tr>
                            <td>Jummah</td>
                            <td>02:45 PM</td>
                            <td>03:15 PM</td>
                        </tr>
                        <tr>
                            <td>Khateeb</td>
                            <td colspan="2">Sh. Ismail Khan</td>
                        </tr>
                        </tbody>
                    </table>
                </div>

            </div>
            <div class="col-xl-5 col-lg-5 col-md-6 col-sm-12 pt-5 pt-md-0">
                <h4 class="text-center pb-3">UPCOMING EVENTS</h4>
                <div class="eventScrollBar scrollbar-dusty-grass card ">
                    <div class="media py-3 " v-for="(n,index) in eventNumber">
                        <h5 class="text-center eventDate mr-3">29 <br> SEP</h5>
                        <div class="media-body" :class="[index !== eventNumber-1 ? 'border-bottom' : '']">
                            <div class="mb-3">
                                <h5 class="mt-0">Media heading</h5>
                                Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin.
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "TimeEvent",
        data(){
            return {
                eventNumber: 9
            }
        }
    }
</script>

<style scoped>
    .prayerTime{
        background-color: #343a40
    }
    .prayerTime .prayerTimeCount {
        color: white;
    }
    .eventScrollBar {
        height: 616px;
        overflow-y: scroll;
    }
    .eventScrollBar .eventDate{
        width: 64px;
        height: 50px;
    }
    .scrollbar-dusty-grass::-webkit-scrollbar-track {
        -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.1);
        background-color: #F5F5F5;
        border-radius: 50px; }

    .scrollbar-dusty-grass::-webkit-scrollbar {
        width: 5px;
        background-color: #F5F5F5; }

    .scrollbar-dusty-grass::-webkit-scrollbar-thumb {
        border-radius: 50px;
        -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.1);
    }
</style>