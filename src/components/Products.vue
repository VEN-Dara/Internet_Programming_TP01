<template>
  <div class="Item-Box" :style="{ backgroundColor: bg }">
    <img class="Img" :src="Img" alt="Product" />
    <div class="itemname">{{ ItemName }}</div>
    <div class="itemnumber">{{ ItemNumber }}</div>
  </div>
</template>

<script>
export default {
  name: "Products",
  props: {
    Img: String,
    ItemName: String,
    bg: String,
    ItemNumber: String,
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Kantumruy+Pro:ital,wght@1,300;1,400;1,500;1,600;1,700&family=Poppins:wght@300;400;500;600;800&family=Quicksand:wght@400;600;700&display=swap");

.Item-Box {
  width: 136px;
  height: 177px;
  margin-right: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  border: 1px solid rgba(129, 177, 61, 1);
  box-shadow: 2px 2px 5px lightgray;
  border-radius: 10px;
}
.Img {
  position: relative;
  bottom: 16px;
  width: 110px;
}
.itemname {
  font-family: "Quicksand", sans-serif;
  position: relative;
  bottom: 15px;
  font-size: 19px;
  color: rgba(37, 61, 78, 1);
  font-weight: 600;
}
.itemnumber {
  font-family: "Quicksand", sans-serif;
  position: relative;
  bottom: 6px;
  font-size: 14px;
  color: rgba(182, 182, 182, 1);
}
</style>
