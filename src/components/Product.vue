<template>
    <div class="main-container">
        <label>Product Title</label>
        <input type="text" placeholder="Enter product title">
        <label>Product Description</label>
        <!-- <textarea id="mytextarea" cols="5" rows="10"></textarea> -->
        <editor
       api-key="no-api-key"
       :init="{
         height: 400,
         menubar: false,
         plugins: [
           'advlist autolink lists link image charmap print preview anchor',
           'searchreplace visualblocks code fullscreen',
           'insertdatetime media table paste code help wordcount'
         ],
         toolbar:
           'undo redo | formatselect | bold italic backcolor | \
           alignleft aligncenter alignright alignjustify | \
           bullist numlist outdent indent | removeformat | help'
        }"
    />
    </div>
</template>

<script>
 import Editor from '@tinymce/tinymce-vue'
  
export default {
    name: 'theProduct',
    components: {
     'editor': Editor
   }
}
</script>


<style scoped>
 .main-container {
        max-width: 900px;
        margin: 30px auto;
        background: rgb(253, 251, 251);
        text-align: left;
        padding: 40px;
        border-radius: 10px;
    }
     label {
        color: #585252;
        display: inline-block;
        margin: 25px 0 15px;
        /* font-size: 0.8em; */
        letter-spacing: 1px;
        font-weight: bold;
    }
     input, textarea {
        display: block;
        padding: 10px 6px;
        width: 100%;
        box-sizing: border-box;
        color: #726d6d;
    }
   
</style>