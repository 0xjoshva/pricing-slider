<template>
<section>
  <div id="heading">
  <h1>Simple, traffic-based pricing</h1>
   <p>Sign-up for our 30-day trial. No credit card required.</p>
   </div>
  <div class="card">
  <div class="top">
    <p id="views">100K PAGEVIEWS</p>
    <p id="price">$16.00 <span>/ month</span></p>
  </div>
<div class="rangediv">
    <input type="range" min="1" max="100" value="50" id="rangeinput">
    </div>
  <div class="range">
      <p class="period">Monthly Billing</p>
      
      <label class="switch">
  <input type="checkbox">
  <span class="slider round"></span>
</label>
      <p class="period year">Yearly Billing</p>
    </div>
    <div class="container-end">
      <ul>
        <li> <img src="../assets/icon-check.svg" alt=""> <p>Unlimited websites</p></li>
        <li><img src="../assets/icon-check.svg" alt=""> <p>100% data ownership</p></li>
        <li> <img src="../assets/icon-check.svg" alt=""> <p>Email reports</p></li>
      </ul>
      <button>Start my trial</button>
    </div>
  </div>
</section>
</template>

<script>
export default {

}
</script>
<style scoped>
section{
  background-image: url(../assets/bg-pattern.svg);
  background-color: var(--verypaleblue);
  width: 100%;
  height: 100vh;
  background-repeat: no-repeat;
  background-size: 100vw 50vh;
  display: flex;
  flex-direction: column;
 justify-content: flex-start;
 align-items: center;
 font-family: 'Manrope', sans-serif; 
}
#heading{
display: flex;
flex-direction: column;
align-items: center;
justify-content: center;
background-image: url(../assets/pattern-circles.svg);
background-repeat: no-repeat;
background-position: center;
width: fit-content;
height: 12rem;
margin-bottom: 3rem;
margin-top: 3rem;
}
#heading h1{
  font-size: 2.2rem;
  color: var(--darkblue);
}
#heading p{
  color: var(--greyishblue);
  font-size: 1.1rem;
  padding-top: .5rem;
}
.card{
  width: 45rem;
  height: 33rem;
  background: var(--white);
  box-shadow: 0px 5px 30px 2px var(--lightgreyishblue1);
  border-radius: 12px;
  padding: 3.5rem;
}
.top{

  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.top #views{
  letter-spacing: 1px;
  font-size: 1.1rem;
  color: var(--greyishblue);
}
#price{
  font-size:2.4rem;
  font-weight: 800;
  color: var(--darkblue);
}
#price span{
  font-size: 1.2rem;
  font-weight: 600;
  color: var(--greyishblue);
  vertical-align: middle;
}
.switch {
  position: relative;
  display: inline-block;
  min-width: 60px;
  min-height: 34px;
}
.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}
.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #ccc;
  -webkit-transition: .4s;
  transition: .4s all ease-in-out;
}
.slider:before {
  position: absolute;
  content: "";
  height: 26px;
  width: 26px;
  left: 4px;
  bottom: 4px;
  background-color: white;
  -webkit-transition: .4s;
  transition: .4s;
}
input:checked + .slider {
 background:linear-gradient(180deg, hsl(236, 72%, 79%), hsl(237, 63%, 64%));
}
input:focus + .slider {
  box-shadow: 0 0 1px hsl(237, 63%, 64%);
}
input:checked + .slider:before {
  -webkit-transform: translateX(26px);
  -ms-transform: translateX(26px);
  transform: translateX(26px);
}
/* Rounded sliders */
.slider.round {
  border-radius: 34px;
}
.slider.round:before {
  border-radius: 50%;
}
.range{
  display: flex;
  width: fit-content;
  height: fit-content;
  align-items: center;
  justify-content: center;
  column-gap: 1.5rem;
  width: 100%;
}
.year::after{
content: "25% discount";
font-size: small;
padding: .4rem .6rem;
border-radius: 26px;
background-color: var();
}
.range p{
    color: var(--lightgreyblue) !important;
}
li{
  list-style-type: none;
  line-height: 2rem;
  display: flex;
  align-items: center;
  column-gap: 1.4rem;
}
li img{
  width: 1rem;
  height: auto;
}
.container-end{
  display: flex;

}
.rangediv{
  padding-top: 3rem;
  padding-bottom: 3rem;
}
#rangeinput{
  width: 100%;

}
</style>