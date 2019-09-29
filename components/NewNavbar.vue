<template>
    <navbar>
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
            <a class="navbar-brand logoImg" href="#">
                <img class="navbarLogo" src="~/assets/images/latestLogo.png" alt="">
            </a>
            <h5 class="font-weight-bold navbarTitle">ISLAMIC community center of Mid Westchester</h5>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav ml-auto text-uppercase">
                    <li class="nav-item mr-2 pt-2 pt-lg-0">
                        <button type="button" class="btn btn-outline-success text-uppercase">Donation</button>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">About Us <span class="sr-only">(current)</span></a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Contact</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Subscribe</a>
                    </li>
                </ul>
            </div>
        </nav>
    </navbar>

</template>

<script>
    export default {
        name: "NewNavbar"
    }
</script>

<style scoped>
    .navbarLogo{
        height: 48px;
        width: 100px;
    }
    .navbarTitle{
        display: none;
    }
    @media (min-width: 768px) {
        .navbarTitle{
            display: inline-block;
        }
    }

</style>