<template>
        <form>
            <div class="form-row">
                <div class="form-group col-md-6">
                    <label for="name">Manufacturer Name</label>
                    <input type="text" class="form-control" id="name" placeholder="Enter Manufacturer Name">
                </div>
            <div class="form-group col-md-6">
            <label for="brand">Manufacturer Brand</label>
            <input type="text" class="form-control" id="brand" placeholder="Enter Manufacturer Brand">
        </div>
    </div>
  
    <div class="form-row">
        <div class="form-group col-md-3">
            <label for="stocks">Stocks</label>
            <input type="text" v-model="stocks" class="form-control" id="stocks">
            {{ stocks }}
        </div>
    <div class="form-group col-md-3">
      <label for="Price">Price</label>
      <input type="number" v-model="price" class="form-control" id="Price">
    </div>
    <div class="form-group col-md-3">     
      <label for="Discount">Discount</label>
      <input type="number" class="form-control" id="Discount">
    </div>
    <div class="form-group col-md-3">
      <label for="Orders">Orders</label>
      <input type="text" class="form-control" id="Orders">
    </div>
  </div>
</form>

</template>

<script>
//General
export default {
    name: 'theInfo',
    data() {
      return {
        stocks: '',
        price: ''
      }
    }
}
</script>


<style scoped>

 form, .form-row{
        max-width: 900px;
        margin: 10px auto;
       background: rgb(253, 251, 251);
        text-align: left;
        padding: 50px;
        border-radius: 10px;
        max-height: 100%
    }
     label {
        color: #585252;
        margin: 25px 0 15px;
        letter-spacing: 1px;
        font-weight: bold;
    }
   
</style>