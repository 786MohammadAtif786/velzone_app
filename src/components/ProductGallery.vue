<template>
    <div class="main-container ">
        <h3 class="border-bottom">Product Gallery</h3>
        <div>
            <h3 class="product_image">Product Image</h3>
            <h4>Add Product Main Image</h4>
            <div class="upload-image">
                <input type="image">
            </div>
        </div>
        <div>
            <h3 class="product_image">Product Gallery</h3>
            <h4>Add Product Gallery Images.</h4>
            <div class="row">
                <div class="col-md-12">
                    <h2><i class='fas fa-cloud-upload-alt'></i></h2> 
                    <div class="file-drop-area">
                        <span class="choose-file-button ">Drop files here</span>
                        <span class="file-message">or cilck to upload</span>
                        <input class="file-input" type="file" multiple>
                    </div>        
                </div>       
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style scoped>


.main-container .border-bottom{
border-bottom: 1px solid rgb(240, 235, 235);
width: 100%;
}
 
.file-drop-area {
  position: relative;
  display: flex;
  align-items: center;
  width: 450px;
  max-width: 100%;
  margin-left: 35%;
  padding: 20px;
  border: 1px dashed rgba(255, 255, 255, 0.4);
  border-radius: 3px;
  transition: 0.2s;
  text-align: center;
 
}
.choose-file-button {
  flex-shrink: 0;
  background-color: rgba(255, 255, 255, 0.04);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 3px;
  /* margin-right: 10px; */
  font-size: 12px;
} 

.file-message {
  font-size: small;
  font-weight: 300;
  line-height: 1.4;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  text-align: center;
}

.file-input {
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 100%;
  cursor: pointer;
  opacity: 0;
}
.product_image {
    font-weight: bold;
}
.upload-image {
    text-align: center;
    height: 40px;
}
/* .mt-100{
    margin-top:100px;
}  */
h2 {
    text-align: center;
}
h3 {
    font-size: medium;
    font-family: 'Courier New', Courier, monospace;
    
}
h4 {
        color: #aaa;
        display: inline-block;
        /* margin: 25px 0 15px; */
        font-size: 1em;
        letter-spacing: 1px;
        font-weight: bold;
}
</style>