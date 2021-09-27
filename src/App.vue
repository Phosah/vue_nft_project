<template>
  <div>
    <router-view/>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Quattrocento+Sans:wght@400;700&family=Roboto:wght@100;300;400;500;700&display=swap');

*,
*:before,
*:after {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
    font-family: 'Roboto', sans-serif;
}

li {
    list-style: none;
}

a {
    text-decoration: none;
}

p {
    font-size: 15px;
}

div,
main,
article,
section,
header,
nav,
footer,
aside {
    display: block;
}
</style>
