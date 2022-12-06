<template>
    <div class="card">
        <div class="card-body">
          <div class="icon">
            <i :class=icon class="s-icon" ></i>
            <div class="s-number">
              <p class="s-tnumber"></p>
            </div>  
          </div>
          <p class="card-text s-text">{{SText}}</p>
          <a :href=link class="s-a">{{SButton}}</a>
        </div>
      </div>
</template>

<script>
export default{
    name : 'ServicesCard',
    props:{
        icon: String,
        SText:String,
        SButton:String,
        SNumber:String,
        link:String
    }
}
</script>