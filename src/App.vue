<template>
  <router-view />
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Manrope:wght@600;800&display=swap");
/* font-family: 'Manrope', sans-serif; */

*,
*::before,
*::after {
  box-sizing: border-box;
}
* {
  margin: 0;
}
html,
body {
  height: 100%;
  font-size: 15px;
}
body {
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
}
img,
picture,
video,
canvas,
svg {
  display: block;
  max-width: 100%;
}
input,
button,
textarea,
select {
  font: inherit;
}
p,
h1,
h2,
h3,
h4,
h5,
h6 {
  overflow-wrap: break-word;
}
#root,
#__next {
  isolation: isolate;
}

:root {
  /* primary */
   --softcyan: hsl(174, 77%, 80%); /*Full Slider Bar */
  --strongcyan: hsl(174, 86%, 45%); /*Slider Background */
  --greyred: hsl(14, 92%, 95%); /*Discount Background */
  --lightred: hsl(15, 100%, 70%); /*Discount Text */
  --paleblue: hsl(226, 100%, 87%); /*CTA Text */

  /* neutral */
  --white: hsl(0, 0%, 100%); /*Pricing Component Background */
  --verypaleblue: hsl(230, 100%, 99%); /*Main Background*/
  --lightgreyishblue1: hsl(224, 65%, 95%); /*Empty Slider Bar*/
  --lightgreyishblue2: hsl(223, 50%, 87%); /*Toggle Background*/
--greyishblue: hsl(225, 20%, 60%); /*Text*/
--darkblue: hsl(227, 35%, 25%); /*Text & CTA Background*/
}
</style>
