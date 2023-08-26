<template>
<body>
    <nav>
   <a @click= "scrollToSection('section1')">Sec1</a>
   <a @click= "scrollToSection('section2')">Sec2</a>
   <a @click= "scrollToSection('section3')">Sec3</a>
   <a @click= "scrollToSection('section4')">Sec4</a>
 </nav>
        <section  id="section1">

        </section>
        <section id="section2">

        </section>
        <section id="section3" class="section3">

        </section>
        <section id="section4" class="section4">

        </section>
        <section id="section5" class="section5">

        </section>
</body>

</template>

<script setup>

import VueScrollTo from 'vue-scrollto';

    const scrollToSection = (sectionRef) =>{
        const element = document.getElementById(sectionRef);
        element.scrollIntoView({behavior:"smooth"})
    }
    
</script>

<style>
*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html,body{
    margin: 0;
    padding: 0;
    height: 100%;
    width: 100%;
    background-color: aqua;
    /* scroll-behavior: smooth;
    scroll-padding: 10rem; */
}
nav{
    top: 0;
    position: sticky;
    background-color: green;
}
.container{
        background-color: orange;
        width: 100%;
        height: 100%;
        margin-top: 0;
}
    #section1{
        height: 720px;
        width: 40rem;
        background-color: red;
    }
    #section2{
        height: 720px;
        width: 40rem;
        background-color: blue;
    }
    .section3{
        height: 109rem;
        width: 40rem;
        background-color: purple;
    }
    .section4{
        height: 720px;
        width: 40rem;
        background-color: red;
    }
</style>