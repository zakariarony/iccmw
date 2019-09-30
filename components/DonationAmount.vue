<template>
  <div class="py-5">
    <div class="row">
      <div class="col-lg-7 mx-auto">
        <div class="bg-white rounded-lg shadow-sm p-5">
          <div>
            <h4 class="pb-2">What type of donation are making?</h4>
            <div>
              <label>
                  <button type="button" class="btn btn-light active">
                <input type="radio" />
                One Time Gift
              </button>
              </label>
              <label >
                  <button type="button" class="btn btn-light">
                <input type="radio" />
                Recuuring Gift
              </button>
              </label>
              <label >
                  <button type="button" class="btn btn-light">
                <input type="radio" />
                Events
              </button>
              </label>
            </div>
          </div>

          <div class="pt-3">
            <h4 class="pb-2">Donation Amount</h4>
            <div>
              <div class="row ">
                <label class="col-sm-4 col-md-3">
                  <button type="button" class="btn btn-lg btn-primary w-100 active">$10,000</button>
                </label>
                <label class="col-sm-4 col-md-3">
                  <button type="button" class="btn btn-lg btn-primary w-100 ">$5,000</button>
                </label>

                <label class="col-sm-4 col-md-3">
                  <button type="button" class="btn btn-lg btn-primary w-100">$2,500</button>
                </label>
                <label class="col-sm-4 col-md-3">
                  <button type="button" class="btn btn-lg btn-primary w-100">$1,000</button>
                </label>
                <label class="col-sm-4 col-md-3">
                  <button type="button" class="btn btn-lg btn-primary w-100">$500</button>
                </label>
                <label class="col-sm-4 col-md-3">
                  <button type="button" class="btn btn-lg btn-primary w-100">$250</button>
                </label>
              </div>
            </div>
          </div>
          <div class="pt-5">
            <span class="pr-2">Other :</span>
            <input placeholder="$" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.btn-primary:not(:disabled):not(.disabled).active{
    color:black;
    background-color: white;
}
</style>