<template>
<body>
    <nav>
        <div class="info">
            <p class="nav-head">Akanimoh Obot</p>
            <p class="email">oakanimoh@gmail.com</p>
            <p class="contact">07012508259</p>
        </div>
        <div class="link">
            <a @click= "scrollToSection('section1')">About Me</a>
            <a @click= "scrollToSection('section2')">Skills</a>
            <a @click= "scrollToSection('section3')">Projects</a>
            <a @click= "scrollToSection('section4')">Recommendations</a>
        </div>
     </nav>
     <div class="container">
         <section  id="section1">
            <img src="../assets/IMG_20220913_013835.jpg" alt="" srcset="">
            <div class="write-up">
                <h1>
                Hi, I'm Akanimoh Obot!
                </h1>
                <p class="write">
                    As a dedicated junior developer with a strong 
                    foundation in computer engineering and proficiency
                    in HTML, CSS, JavaScript, Vue.js, and Node.js, 
                    I am seeking an opportunity to contribute to 
                    dynamic projects and continue learning in a
                    collaborative software development environment.
                </p>
            </div>
            
        </section>
        <section id="section2">
            <h2>Skills</h2>
            <div class="all-boxes">
                <div class="box">

                </div>
                <div class="box">

                </div>
                <div class="box">

                </div>
                <div class="box">

                </div>
                <div class="box">

                </div>
                <div class="box">

                </div>
                <div class="box">

                </div>
            </div>
        </section>
        <section id="section3">
            <h2>Projects</h2>
            <div class="all-project">
                <div class="project">
                    <div class="project-head">
                        Newsletter Project
                    </div>
                    <li>
                        Implemented user authentication and CRUD functionality for blog posts
                    </li>
                </div>
                <hr>
                 <div class="project">
                    <div class="project-head">
                        Space-web Project
                    </div>
                    <li>
                      Utilized Vue.js to build dynamic components, enabling real-time updates
                    </li>
                </div>
                <hr>
                 <div class="project">
                    <div class="project-head">
                        Dojo-Blog
                    </div>
                    <li>
                        Developed a blogging platform using Vue.js 
                    </li>
                </div>
            </div>
        </section>
        <section id="section4">
            <h2>Recommendations</h2>
                <div class="hold-top">
                    <div class="holders">
                        <p class="holders-p">
                        "Lorem ipsum dolor sit amet, consectetur adipisicing 
                        elit. Optio dolorem repellendus hic magni fuga molestiae 
                        iste aut deleniti eum sit. Dolorum, corrupti perspiciatis 
                        dolorem incidunt totam aliquid repellendus a maiores 
                        mollitia fugiat. Placeat consectetur quisquam delectus 
                        praesentium dicta hic nostrum fugiat nemo voluptas, 
                        omnis ea accusantium eveniet, est architecto quis."
                        </p> 
                    </div>
                    <div class="holders">
                        <p class="holders-p">
                        "Lorem ipsum dolor sit amet, consectetur adipisicing 
                        elit. Optio dolorem repellendus hic magni fuga molestiae 
                        iste aut deleniti eum sit. Dolorum, corrupti perspiciatis 
                        dolorem incidunt totam aliquid repellendus a maiores 
                        mollitia fugiat. Placeat consectetur quisquam delectus 
                        praesentium dicta hic nostrum fugiat nemo voluptas, 
                        omnis ea accusantium eveniet, est architecto quis."
                        </p> 
                    </div>
                    <div class="holders">
                        <p class="holders-p">
                        "Lorem ipsum dolor sit amet, consectetur adipisicing 
                        elit. Optio dolorem repellendus hic magni fuga molestiae 
                        iste aut deleniti eum sit. Dolorum, corrupti perspiciatis 
                        dolorem incidunt totam aliquid repellendus a maiores 
                        mollitia fugiat. Placeat consectetur quisquam delectus 
                        praesentium dicta hic nostrum fugiat nemo voluptas, 
                        omnis ea accusantium eveniet, est architecto quis."
                        </p>  
                    </div>
                </div>
                <div class="hold-bottom">
                    <form action="">
                 
                                 <span>Leave a Recommendation</span><br>
                            
                                <input type="text" placeholder="Name (Optional)" class="name">
                                <textarea name="" id="" cols="30" rows="10" class="message" placeholder="Message"></textarea>
                            
                             <button type="submit">Submit</button>
                    </form>
                </div>
           
        </section>
     </div>
        
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
    align-items:  center;
    justify-content:  center;
}

html,body{
    margin: 0;
    padding: 0;
    height: 100%;
    width: 100%;
    background-color: aqua;
    scroll-behavior: smooth;
    scroll-padding: 8rem; 
    align-items: center;
    justify-content: center;
}
nav{
    display: flex;
    justify-content: space-between;
    padding: 1rem 1rem 0rem 1rem;
    top: 0;
    position: sticky;
    background-color: rgb(38, 36, 182);
    color: white;
}
.info{
    padding: 1rem 1rem 1rem 1rem;
}
.link{
    background-color: red;
    margin: 0.5rem;
}
.link a{
    margin: 1rem 1rem 1rem 3rem;
}
.container{
        display: inline-block;
        justify-content: center;
        align-items: center;
        background-color: green;
        width: 100%;
        height: 100%;
        margin-top: 0;
        
}
    #section1{
        display: flex;
        height: 580px;
        width: 100%;
        background-color: red;
    }
    #section1 >img{
        height: 28rem;
        width: 28rem;
        margin: 3rem 1rem 1rem 4rem;
    }
    #section1 .write-up{
        background-color: white;
        margin: 8rem 1rem 1rem 1rem;
        width: 48rem;
        height: 20rem;
    }
    #section1 h1{
        font-size: 3rem;
        font-weight: 500;
        margin: 3rem 0rem 2rem 0rem;
    }
     #section1 .write{
         padding-right:1rem ;
     }

    #section2{
        height:580px;
        width: 100%;
        background-color: orange;
    }
     h2{
        color: purple;
        font-size: 2rem;
        margin-left: 2.5rem;
    }
    .all-boxes{
        display: grid;
        grid-template-columns: auto auto auto auto;
        height: 600px;
        width: 100%;
        background-color: rgb(137, 94, 14);
    }
    .box{
        height:12rem;
        width: 14rem;
        background-color: aqua;
        margin: 1rem 2rem 2rem 1rem;
         box-shadow: 1px 1px 1px 0 rgba(154, 160, 185, 0.05),
         1px 1px 15px rgba(0 ,0, 0, 0.3);
    }

    #section3{
        height: 580px;
        width: 100%;
        background-color: rgb(227, 186, 227);
        align-items: center center;
        justify-content: center center;
        text-align: center ;
    }
     #section3 h2{
         text-align: left;
     }
     #section3 .all-project{
         display: inline-block;
        background-color: white;
         margin: 0;
        padding: 0;
        height: 33rem;
        width: 80rem;
        align-items: center;
        justify-content: center;
        
    }
    .project{
        display: inline-block;
        height: 6rem;
        width: 70rem;
        text-align: left;
        margin: 1.5rem;
        background-color: blue;
    }
    .project .project-head{
        font-weight: bold;
        margin: 1rem;
    }
    .project li{
        margin-left: 2rem;
    }
     hr{
         display: inline-block;
         text-align: center;
         margin:1rem 2rem 1rem 1rem ;
         height: 0.2px;
         width: 70%;
    }
#section4{
    height: 880px;
    width: 100%;
    background-color: lawngreen;
}

.hold-top{
    display: flex;
    height: 20rem;
    background-color: aquamarine;
}
.holders{
    padding: 0;
    display: flex;
    width: 25rem;
    height: 12rem;
    background-color: lightgrey;
    border-radius: 20px 20px;
    border: 2px solid rgba(60, 55, 55, 0.422);
    margin: 0rem 1rem 4rem 1rem;
}
.holders-p{
    font-family: cursive;
    font-style: italic;
    line-height: 20px;
}

.hold-bottom{
    background-color: lightslategray;
    display: inline-block;
    height: 34rem;
    width: 100%;
    justify-content: center;
    align-items: center;
    text-align: center;
}
form{
     display: inline-block;
    background-color: yellow;
    justify-content: center;
    align-items: center;
    text-align: left;
    width: 49rem;
}

 span{
     margin: 1rem;
     font-size: 30px;

}
.name{
     margin: 1rem;
     width: 46rem;
}
.message{
    padding: 0;
     margin: 1rem;
     width: 46rem;
     height: 12rem;
} 
.message::placeholder{
    font-size: 16px;
}
button{
     display: flex;
     margin: auto;
      width: 11rem;
     height: 3.5rem;
     margin-top: 4rem;
     border: 2px solid purple;
     font-size: 18px;
    font-weight: bold;
    color: purple;
     border-radius:6px ;
}
button:hover{
    background-color: rgb(218, 57, 218);
    color: beige;
}
</style>